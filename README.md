FPGA-project-1
Authors: 108321058  108321055
Input/Output unit:
1.圖中有六個led輸出，最右側為gameover輸出，若為1，則遊戲結束，左側五個為發射器的剩餘發射次數。  
![image](https://github.com/Jeremyngu123/Final-Project/blob/main/LINE_P2021115_110401.jpg)
2.圖中為積分led輸出。
![image](https://github.com/Jeremyngu123/Final-Project/blob/main/LINE_P2021115_110402.jpg)
3.圖中為按下重置按鈕之後的畫面，即開始畫面，隨後便是遊戲時間
![image](https://github.com/Jeremyngu123/Final-Project/blob/main/LINE_P2021115_110359.jpg)

功能說明：
玩家控制一個球，在障礙物掉落的同時要避開這些障礙物，積分隨著時間的增加而增加。

module finalfantasy（input CLK,input CLEAR//重置,input reg[2:0] buttonREG//玩家左右发射,output reg[3:0] COMM//控制亮燈排數,output reg [0:7]R //紅色燈,output reg [0:7]G //綠色燈, output reg [0:7]B //藍色燈,output reg[3:0] Segcom//控制記分亮燈排數,output reg[6:0] SegDiaplay//記錄分數，output reg GameOver//结束时会亮的灯,output reg[4:0] biubiubiu//弹药数量）

4-bit SW-s1 玩家左边  
         s2 玩家发射  
         s3 玩家右边  
         s4 重置  
         
![影片(試玩)](https://drive.google.com/file/d/1uwQUay48OgClo0YOdfmWXQ1D2nqbDoOs/view?usp=sharing)  

![影片(講解)](https://drive.google.com/file/d/1pd37GGJBwt0EYczG0rwtPW2_kDi19Ulv/view?usp=sharing)
