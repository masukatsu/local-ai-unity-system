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
# ChromeDB
　ChromeDBは基本的に会話履歴から必要な情報を参照するために使います
# 概要
　このローカルAI環境では自分のパソコンのスペック限界
 GPU：RTX3050(4GB)    CPU：32GB
 の上限のもとに作成しました
 まず記憶機能としては会話を丸々覚えるとAIの性能が落ちる危険性などもあるため
 会話履歴として過去の会話を参照する仕組みにしました
 

 
