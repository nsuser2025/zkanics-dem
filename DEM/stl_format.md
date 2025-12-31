<p>
物体形状の表現を小さな三角形ポリゴンメッシュの集合で行う.
Fig. 1のように反時計回りで3頂点の座標とメッシュの法線ベクトル ${\bf n}$
が記録されている.
ただ、多くのソフトではfacet normalは無視され, 
3点の座標から法線ベクトルを再計算することが多い.
</p>

<figure style="text-align: center;">
<img src="https://raw.githubusercontent.com/nsuser2025/zkanics-dem/main/DEM/STL.png" alt="GELDART_CLASS" width="200">
<figcaption style="text-align:center;">Fig. 1 STLフォーマット </figcaption>
</figure>

<p>
</br>
<span style="color:gray">
solid 任意の文字列 </br>
</span>  
<span style="color:blue">
facet normal x成分 y成分 z成分 </br>
outer loop </br>
vertex x y z </br>
vertex x y z </br>
vertex x y z </br>
end loop </br>
end facet </br>
</span> 
<span style="color:gray">
endsolid </br></br>
</span>  
青文字の箇所がメッシュの枚数分書かれている.
</p>
