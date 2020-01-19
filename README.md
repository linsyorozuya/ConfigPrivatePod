# ConfigPrivatePod

在一个项目实施组件化方案之前，我们需要做一个准备工作，建立自己的私有Pod源和快手工具脚本的配置：

1. 先去开一个repo，这个repo就是我们私有Pod源仓库
2. pod repo add [私有Pod源仓库名字] [私有Pod源的repo地址]
3. 创立一个文件夹，例如Project。把我们的主工程文件夹放到Project下：~/Project/MainProject
4. 在~/Project下clone快速配置私有源的脚本repo：git clone git@github.com:casatwy/ConfigPrivatePod.git
5. 将ConfigPrivatePod的template文件夹下Podfile中source 'https://github.com/ModulizationDemo/PrivatePods.git'改成第一步里面你自己的私有Pod源仓库的repo地址
6. 将ConfigPrivatePod的template文件夹下upload.sh中PrivatePods改成第二步里面你自己的私有Pod源仓库的名字
