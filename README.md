# local-ai-unity-system
ローカルAI、Docker、Unity、HTTP、ChromeDBを使ったローカルAI環境
# ベースにローカルAI2種類
--会話AI｛Phi-3-mini-4k-instruct-q4｝
--生成AI｛Qwen2.5-Coder-3B-4bit｝
# Dockerコンテナの使用
  Dockerでは3つのコンテナを立てました
  --fastAPI｛司令塔の役割｝
  --phi3｛会話AI｝
  --qwen｛生成AI｝
# Unity
　Unityは主にUIとしてだけ使用しています
 例えばこんにちはというリクエストをHTTP通信でDockerに送り
 レスポンスをHTTP通信で受信し表示するだけのもの
# 一連の流れ
　このローカルAI環境では自分のパソコンのスペック限界
 GPU：RTX3050(4GB)    CPU：32GB
 の上限のもとに作成しました
 会話AIと生成AIとで二つ別々である理由は
 
