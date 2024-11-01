## 怕以後自己忘記怎麼包的指令集

創建虛擬環境
conda create -n elf python=3.9 

啟動虛擬環境
conda activate lef_2 

安裝套件
pip install Pillow pyinstaller

安裝套件以設置核心
pip install ipykernel
python -m ipykernel install --user --name=elf --display-name "Python (elf)"

安裝注音轉譯套件
pip install pypinyin

安裝封包套件
pip install pyinstaller

轉為exe執行檔
pyinstaller --onefile --noconsole --hidden-import=PIL --add-data "elffont-rock.otf;." --add-data "elffont-fern.otf;." Elf_translator.py
