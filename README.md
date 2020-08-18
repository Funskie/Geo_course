# 環境安裝介紹
## 下載課程檔案
* 若有安裝`git`可以直接`clone`
   
   `git clone https://github.com/Funskie/Geo_course.git`
* 沒有安裝`git`請直接下載zip檔並解壓縮

## 利用 `Anaconda` 安裝環境
### [Anaconda](https://www.anaconda.com/distribution/)
* 點選上面連結下載符合OS的**PYTHON3**安裝檔並執行*PATH要打勾*
* Anaconda指令介紹
    * 檢視目前環境列表

        `conda env list`
    * 建立虛擬環境

        `conda create -n <env name>`
    * 啟動虛擬環境

        `conda activate <env name>`
    * 離開虛擬環境

        `conda deactivate` 
    * 複製虛擬環境

        `conda create -n <new env name> --clone <old env name>`
    * 刪除虛擬環境

        `conda env remove -n <env name>`
    * 安裝module在目前環境

        `conda install <module name>` 
    * 刪除虛擬環境內的module
    
        `conda remove -n <env name> <module name>`
* 建立虛擬環境

    `conda create -n py36 python=3.6 anaconda`
* 進入虛擬環境

    `conda activate py36`

### 安裝套件
* 記得確認是否在虛擬環境內
* 安裝相關套件

    `anaconda search -t conda xgboost`
    
    `conda install -c anaconda py-xgboost`

### [Visual Studio Code (option)](https://code.visualstudio.com/)
* Visual Studio Code，是一款Microsoft開發的輕量、跨平台的程式碼編輯器。雖然他不是IDE，但是搭配上各種社群 & 官方開發的Plugins，可以有很方便的開發體驗。

### Jupyter Notebook 
* 理論上`Anaconda`會幫我們把這些都裝好，我們只要在terminal內下指令就會自動執行
    
    `jupyter notebook` 

    如果沒有安裝則先在虛擬環境內下

    `conda install jupyter`

    `jupyter notebook` 
