# 噪点生成的一些研究
噪点生成一般通过几个参数来生成随机的图像，换句话说 其实 就是一个属于随机发生器
构造随机发生器，第二步是插值，第三步是叠加。

## 一些噪点共有的属性
1 .octaves:定义要处理的八度音阶数。这个值越大，生成的噪点越密集，可以看成是地形会从丘陵变成石林

1 .每个你所叠加的噪声函数就是一个倍频，每一个噪声函数是上一个噪声函数的两倍频率
2 .我认为叠加每次的不同的频率是为了让图像在原有的噪声函数的基础上增加更多的细节信息。
2 .persistence:定义持久性级别（默认为0.8）.感觉是明暗对比度。

1 .属于柏林噪声的属性
2 .持续度越大，图像更加混乱，对比更加突出，能够看出更多细节
image.png
3 .animationSpeedFactor：获取或设置动画速度因子（默认值为 1)变化的速度，绝对值越大，噪点图变化速度越快
4 .brightness:获取或设置一个介于0和1之间的值，该值指示纹理的总体亮度（默认值为0.2）k看来这个才是亮度

'''

    ground.material=mat

            mat.disableLighting = true;
            mat.backFaceCulling = false;
            let noiseTexture=new BABYLON.NoiseProceduralTexture('perlin',256,scene)
            // 名字
            // 定义纹理的大小，默认是256
            // scene
            // fallbackTexture:定义无法创建NoiseProceduralTexture时要使用的纹理
            // generateMipMaps: boolean:定义是否必须生成mipmap（默认为true）

            
            mat.emissiveTexture=noiseTexture
//这样会给一个物体加上最基础的噪点纹理，并且还是动态变化的
'''

作者：skoll

链接：https://www.jianshu.com/p/891d9d3ce374

来源：简书

著作权归作者所有。商业转载请联系作者获得授权，非商业转载请注明出处。


一些噪点种类：
1 .白噪点
2 .柏林噪点
3 .turbulence noise 湍流噪声
4 .ridge noise
6 .Domain Warping
7 .Voronoi Nose
8 .Curl Noise


接下来就尝试实现一下
doit

