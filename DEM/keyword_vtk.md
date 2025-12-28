<p>
GRANULARの結果をParaViewで可視化するためには, dump vtkを用いる.</br></br>
dump 1 all vtk 100 movie_*.vtk id type radius mass x y z </br></br>
LAMMPSのdump vtkが時系列出力に対応していないため, このコマンドに記載の "_*" とすることによって,
各時刻ごとに個別のvtkファイルが生成されるようになる.
各vtkファイルには１フレームのトラジェクトリが記載される.
boundingBox.vtkファイルも同時に生成されるがsimulation boxの情報は記載されているが,
regionの詳細な情報は書かれていないのでParaViewで読み込んでもregionで指定した
容器形状の表示はできない.
</p>
