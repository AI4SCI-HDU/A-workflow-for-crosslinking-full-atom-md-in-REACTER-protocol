# 需要的工具
Gaussian·GaussView·gromacs·lammps·gro2lam·automapper·vscode·cgenff
gro2lam仅能在Ubuntu的图形化界面使用

# 流程
Gaussian·GaussView-建模、结构优化-得到mol2文件
cgenff-使用mol2文件得到gromacs中的力场
gro2lam-转换至lammps文件
automapper-进行力场清洗-生成反应模板