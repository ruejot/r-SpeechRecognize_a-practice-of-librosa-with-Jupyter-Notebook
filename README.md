# python_語音辨識練習
基於tensorflow之公開dataset作單詞語音識別。過程中使用Librosa與Keras操作。  
於Jupyter Notobook環境下進行

來源 [Tensorflow](https://www.tensorflow.org/tutorials/sequences/audio_recognition#tensorboard "Simple Audio Recognition")、[SimpleSpeechRecognizer](https://github.com/manashmndl/DeadSimpleSpeechRecognizer "git")

## Dataset
dataset是在Tenseoflow_Tutorials中的Simple Audio Recognition所提及。  
下在連結於Speech Commands dataset。

## MFCC
其中從.wav音訊檔提取MFCC特徵是使用Librosa實現。  
並存至.npy以供之後訓練。

## 辨識學習
這裡提取資料集其中的4項單詞作為分類目標{''、'one'、'two'、'three'}。  
在訓練前，有先對各項擷取前2個音檔出來作為手動驗證目標，存在testSample目錄下。  
其餘的使用sklearn套件和Kersa作訓練/測試以完成模型。

---
### Index
[Mel-Frequency Cipstal Coefficients](https://zh.wikipedia.org/wiki/%E6%A2%85%E7%88%BE%E5%80%92%E9%A0%BB%E8%AD%9C "MFCC")
