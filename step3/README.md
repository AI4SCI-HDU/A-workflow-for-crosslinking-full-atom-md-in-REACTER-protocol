# Step3
## 1.将top文件改为itp文件
删除所有include和分子拓扑后的所有内容
如果有计算resp电荷，在此一并修改itp文件的电荷

## 2.将pdb文件转换成gro文件，加入box信息
```yaml
gmx editconf -f PA1_gmx.pdb -o PA1_gmx.gro -box 5 5 5
```

## 3.合并力场文件
将XX_ffbonded.itp合并至力场ffbonded.itp
使用vs code可以很方便检查重复行

## 4.编写反应前体系的gro文件
将两个反应分子复制到同一个gro即可

## 5.编写体系的top文件