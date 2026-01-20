# Step4
由于gro2lam程序缺乏鲁棒性，对输入文件的格式有较高的要求
需要对先前简单编写的gro格式进行规范，使用gmx程序直接输出即可
```yaml
gmx grompp -f ions.mdp -c pre1.gro -p pre1.top -o tra.tpr -maxwarn 10
gmx genion -s tra.tpr -o pre1.gro
```