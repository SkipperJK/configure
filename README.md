# Python

## LAN access Jupyter 
```bash
# generate config file
jupyter-notebook --generate-config
# set access jupyter password 
jupyter-notebook password
```
Modify the jupyter config file:
- 1. 命令操作
```bash
echo "c.ConnectionFileMixin.ip = '0.0.0.0'" >> ~/.jupyter/jupyter_notebook_config.py
echo "c.NotebookApp.ip = '0.0.0.0'" >> ~/.jupyter/jupyter_notebook_config.py
```
- 2. 手动修改配置文件
`vim ~/.jupyter/jupyter_notebook_config.py`
修改/添加:
	c.ConnectionFileMixin.ip = '0.0.0.0'"
	c.NotebookApp.ip = '0.0.0.0'" 

