# wpf ドラッグ移動サンプル

MVVM Bindingサンプル。

- WPF / .NET 6.0 
- MVVMライブラリ未利用。MvvmUtilsフォルダに単純なものを用意。
- `RectInfo`というデータクラスでRectangleを管理
- Canvas上のUIElementをドラッグ移動させるとDataGridに反映。
- 逆方向も反映



![sample](/img/a.gif) 

### 更新

サンプルなのでより平易になるようにファイル構成などを変更。

- フォルダをやめて平坦に。
- 削除ボタンをコマンド化。
- ファイル数削減。
- DataGridをMainWindow内に直接配置。これにより`SelectedItem`プロパティをDataGridとCanvas間で直接Bindingするように変更、ViewModel管理をやめた。
- データ管理(Model)をMyDataクラスに分離
