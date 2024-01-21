    Point（点）:
        a, b, c, ... 是点的变量名称。

        Midpoint (中点):
            midpoint o b c 表示线段bc的中点o。
        例子1：
            o = midpoint o b c
            这表示o是线段bc的中点。其中midpoint可能是一个函数，用于计算线段的中点。



    Segment（线段）:
        a b 表示线段ab。
    
        g1, g2, ... 是线段的变量名称。

        on_bline
            
        例子1： 存在一点T 使得 TB=TD ，TC=TE 
            t = on_bline b d, on_bline c e;
        例子2： 且直线AC上的点X满足CX=BX
            x = on_bline b c, on_line a c

        on_tline : 垂直 

        例子1：过园i上D作垂线 DR 垂直 EF ，交园i于R        
        r = on_tline r d e f, on_circle r i d;



    Triangle（三角形）:
        a b c 表示三角形abc。

        例子：
          a b c = triangle a b c
          这表示a, b, 和 c 是三角形的三个顶点，并且triangle a b c可能是一个命令或函数，用于定义或表示一个三角形。

        Ortho-Center (垂心):
            orthocenter h a b c 表示三角形abc的垂心h。

        Incenter (内心):
            incenter2 t1 t2 t3 i a b c 表示三角形abc的内心i，t1, t2, t3是i与边的交点。r = on_tline r d e f, on_circle r i d;

        Foot (垂足):
            foot h1 a b c 表示从a到bc的垂足h1。

    Circle（圆）:
        circle o1 b m r 表示通过点b、m和r的圆o1。            
            例子： 
                1) Circle Through (通过点的圆):
                    circle o1 b m r 表示通过点b、m和r的圆o1。

                2) o1 = circle o1 b m r; o2 = circle o2 c n r
                    这表示圆o1是三角形 bmr外接圆 。其中circle可能是一个函数，用于定义一个圆。
                    o1类似，这表示圆o2以三角形 cnr外接圆。

        on_circle : on_circle m o b 表示点m、b 在圆o上 

            1) on_circle 表示某点在圆上。例如，on_circle m o b 表示点m、b 在圆o上 .

            2) m = on_circle m o b, on_line m a b
            这表示点m位于以o为圆心、b为圆上的一个点并与直线a b相交的圆上。
                其中on_circle和on_line可能是函数，用于确定一个点是否在某个圆上或在某条直线上。

            3) n = on_circle n o b, on_line n a c
            这表示点n位于以o为圆心、b为圆上的一个点并与直线a c相交的圆上。







    Angle (角):

        angle_between a b c 表示直线ab与直线bc之间的夹角。

         
        angle_bisector:
            表示角b的角平分线r。
            例子：
            r = angle_bisector r b a c, angle_bisector r m o n
            这表示点r是角BAC的平分线与角MON的平分线的交点。其中angle_bisector可能是一个函数，用于计算角的平分线。

        eqangle2： 
            例子： a = eqangle2 b t e;  角ABT =角TEA
        
        on_aline： 角度相等
            例子1： 线段AC上的点E满足∠ADE=∠BCD
                e = on_aline d a d c b, on_line a c; 
            例子2： 线段AB上的点F满足∠FDA=∠DBC
                f = on_aline d a d b c, on_line a b

        eqangle3：
            例子1： P1在PB1上， 使得∠PP1C=∠BAC ； Q1在A1Q上 ，∠CQ1Q = ∠CBA
                p1 = on_line p b1, eqangle3 p c a b c; q1 = on_line q a1, eqangle3 c q b c a 



    Plane Line (平面线):
        c, d, ... 是平面线的变量名称。

    Line (直线):
        e, f, ... 是直线的变量名称。



    
 d e f i = incenter2 d e f i a b c

    Reflect (反射):
        reflect x1 h1 t1 t2 表示点t1在直线h1上的反射点x1。



    Congruent (全等的):
     线段相等： 
       cong o p o q
     例子：证明 ep=eq 
        cong 表示两个几何对象是全等的。例如，cong e p e q 表示e、p和q是全等的。

    Collinear (共线的):

    coll p b c 表示点p、b和c共线。
        例子：
        p = on_circle p o1 r, on_circle p o2 r ? coll p b c
        这表示点p位于外接圆o1和外接圆o2上，并且判断点p、b和c是否共线。其中on_circle、coll p b c可能是一些函数，分别用于确定一个点是否在某个圆上和判断三个点是否共线。



    Parallel (平行的):

    par a b c d 表示直线ab与直线cd平行。

    Parallel to (与...平行的):

    on_aline p b c a b d 表示直线p与直线a b平行。




on_line、on_circle、on_pline、on_bline：表示与线、圆、抛物线或线段相切。可能的含义包括：确定切点的位置。






    o1 = circle o1 b m r
        这表示外接圆o1以线段bm为直径，并且经过点r。其中circle可能是一个函数，用于定义一个圆。

    o2 = circle o2 c n r
        与o1类似，这表示外接圆o2以线段cn为直径，并且经过点r。


# 2022IMO平面几何试题
    https://zhuanlan.zhihu.com/p/540810705

    令 为一凸五边形满足 , 假设在 内部存在一点 使得 且 . 令直线 分别与直线 和 交于点 和 , 假设 在同一直线上按照此顺序排列. 令直线 分别与直线 和 交于点 和 , 假设 在同一直线上按照此顺序排列. 求证: 四点共圆.
    
    translated_imo_2022_p4

        b c = segment; d = free; e = eqdistance d b c; t = on_bline b d, on_bline c e; a = eqangle2 b t e; p = on_line a b, on_line c d; q = on_line a b, on_line c t; r = on_line a e, on_line c d; s = on_line a e, on_line d t ? cyclic p q r s

# 2021 IMO第三题
https://zhuanlan.zhihu.com/p/397168202

translated_imo_2021_p3
a b c = triangle; d = angle_bisector b a c; e = on_aline d a d c b, on_line a c; f = on_aline d a d b c, on_line a b; x = on_bline b c, on_line a c; o1 = circle a d c; o2 = circle e x d; y = on_line e f, on_line b c ? coll o1 o2 y


# 2019年国际数学奥林匹克竞赛IMO第六题

 https://www.zhihu.com/question/336975868/answer/764160402?utm_id=0

 translated_imo_2019_p6
a b c = triangle a b c; d e f i = incenter2 d e f i a b c; r = on_tline r d e f, on_circle r i d; p = on_line p r a, on_circle p i d; o1 = circle o1 p c e; o2 = circle o2 p b f; q = on_circle q o1 p, on_circle q o2 p; t = on_line t p q, on_line t i d ? perp a t a i

# 019年国际数学奥林匹克竞赛IMO2 
translated_imo_2019_p2
a b c = triangle; a1 = on_line b c; b1 = on_line a c; p = on_line a a1; q = on_line b b1, on_pline p a b; p1 = on_line p b1, eqangle3 p c a b c; q1 = on_line q a1, eqangle3 c q b c a ? cyclic p q p1 q1

https://zhuanlan.zhihu.com/p/454888089
在三角形ABC中，B1在CA上，A1在BC上。 P在AA1上，Q在BB1上， PQ//AB, P1在PB1上， 使得∠PP1C=∠BAC ； Q1在A1Q上 ，∠CQ1Q = ∠CBA。证明：PQP1Q1四点共圆




# 2009年IMO第二题-几何
https://zhuanlan.zhihu.com/p/430362495?utm_id=0

translated_imo_2009_p2
m l k = triangle m l k; w = circle w m l k; q = on_tline q m w m; p = mirror p q m; b = mirror b p k; c = mirror c q l; a = on_line a b q, on_line a c p; o = circle o a b c ? cong o p o q
O是三角形ABC的外心，P,Q分别是边CA，AB上的点，K,L,M分别是BP,CQ,PQ上的中点，KLM的外接圆与PQ相切，证明：OP=OQ