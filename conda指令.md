# conda指令

## 1.创建新环境

```
conda create -n your_env_name python=X.X 
# 或
conda create --name your_env_name python=X.X
```

## 2.激活环境

```
conda activate your_env_name
```

## 3.退出当前虚拟环境

```
conda deactivate # Windows环境
```

## 4.删除某个虚拟环境

```
conda remove -n your_env_name --all
# -n即--name
```

## 5.复制某个虚拟环境

```
conda create --name new_env_name --clone old_env_name 
```

## 6.环境查询

查看安装了哪些包：

```
conda list
```

查看当前有哪些虚拟环境：

```
conda env list
# 或
conda info --envs
```

查询版本

```
python --version
conda --version
```

更新conda

```
conda update conda
```

查询conda环境详细信息

```
conda info
```

## 7.包的安装、删除、升级

```
conda install [package] 
# 如：conda install numpy
# 指定包版本：conda install xlrd=1.2.0 (注意是单等于号）
# 也可以使用pip install安装 pip install xlrd==1.2.0 (注意是双等于号）
# 查看可用的版本：pip install spyder==*

conda remove [package] 
# 请注意：并非conda uninstall
# pip指令下才有 pip uninstall

conda update [package]
# conda update --all 升级所有包
```

## 8.分享/备份环境

一个分享环境的快速方法就是给他一个你的环境的`.yml`文件。

首先激活到要分享的环境，在当前工作目录下生成一个`environment.yml`文件。

```
conda env export > environment.yml
```

对方拿到`environment.yml`文件后，将该文件放在工作目录下，可以通过以下命令从该文件创建环境。

```
conda env create -f environment.yml
```

## 9.镜像源

查看

```
conda config --show channels
```

添加

```
conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/free
conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/main
conda config --set show_channel_urls yes
 
# conda config --set show_channel_urls yes的意思是从channel中安装包时显示channel的url，这样就可以知道包的安装来源了。
```

移除

```
conda config --remove channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud/conda-forge/
```

## 10.清理

删除没有用的包

```
conda clean -p     
```

删除tar包

```
conda clean -t     
```

删除所有的安装包及cache

```
conda clean -y --all 
```

