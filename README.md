# aframe-gaussian-splattingに簡易的なレイキャスト機能を追加したもの
https://github.com/user-attachments/assets/2a65c389-c718-4603-809e-60b0ea2e26c1

aframe-gaussian-splattingはガウシアンスプラフティングの3dモデルを描画する機能しか提供されていないが、当たり判定が欲しかったので簡易的に実装。
以下の挙動でうごいてます。
1. splatから点の座標と透明度を抽出 ※1
2. ※1から透明度が大きい点を削除
3. クリック方向にレイを飛ばして指定サイズの box を順に配置 ※2
4. ※2の中の点群の数が10個以上存在する場合に赤いボックスを表示。これが当たり判定

<img width="1248" height="684" alt="image" src="https://github.com/user-attachments/assets/672d2f41-050b-4674-ad74-1737e9e1b710" />
