extensions [nw]

breed [nodes node]
nodes-own
[ID
  ;; this is used to mark turtles we have already visited
  explored?

 short
  short0
  short_aa short_ab short_ac short_ad short_ae short_af short_ag short_ah short_ai short_aj short_ak short_al short_am short_an short_ao short_ap short_aq short_ar short_as short_at short_au short_av short_aw short_ax short_ay short_az
  short1
  short_ba short_bb short_bc short_bd short_be short_bf short_bg short_bh short_bi short_bj short_bk short_bl short_bm short_bn short_bo short_bp short_bq short_br short_bs short_bt short_bu short_bv short_bw short_bx short_by short_bz
  short2 shortc
  short3 shortd
  short4 shorte
  short5 shortf
  short6 shortg
  short7 shorth
  short8 shorti
  short9 shortj
  short10 shortk
  short11 shortl
  short12 shortm
  short13 shortn
  short14
  short_oa short_ob short_oc short_od short_oe short_of short_og short_oh short_oi short_oj short_ok short_ol short_om short_on short_oo short_op short_oq short_or short_os short_ot short_ou short_ov short_ow short_ox short_oy short_oz
  short15 shortp
  short16 shortq
  short17 shortr
  short18 shorts
  short19 shortt
  short20
  short_ua short_ub short_uc short_ud short_ue short_uf short_ug short_uh short_ui short_uj short_uk short_ul short_um short_un short_uo short_up short_uq short_ur short_us short_ut short_uu short_uv short_uw short_ux short_uy short_uz
  short21 shortv
  short22 shortw
  short23 shortx
  short24 shorty
  short25
  short_za short_zb short_zc short_zd short_ze short_zf short_zg short_zh short_zi short_zj short_zk short_zl short_zm short_zn short_zo short_zp short_zq short_zr short_zs short_zt short_zu short_zv short_zw short_zx short_zy short_zz

   path path0 path1 path2 path3 path4 path5 path6 path7 path8 path9 path10 path11 path12 path13 path14 path15 path16 path17 path18 path19 path20 path21 path22 path23 path24 path25
  j

  cluster0
  cluster1
  cluster2
  cluster3
  cluster4
  cluster5
  cluster6
  cluster7
  cluster8
  cluster9
  cluster10
  cluster11
  cluster12
  cluster13
  cluster14
  cluster15
  cluster16
  cluster17
  cluster18
  cluster19
  cluster20
  cluster21
  cluster22
  cluster23
  cluster24
  cluster25


]



globals
[
  component-size          ;; number of turtles explored so far in the current component
  giant-component-size    ;; number of turtles in the giant component
  giant-start-node        ;; node from where we started exploring the giant component
  pathlength              ;; sum of the path lengths between all nodes in the network
  meancluster             ;; mean cluster of the network
  pathposs
  ]


;;;;;;;;;;;;;;;;;;;;;;;;
;;; Setup Procedures ;;;
;;;;;;;;;;;;;;;;;;;;;;;;


to setup
  clear-all
  ask patches [
    set pcolor white
  ]

create-nodes 1[;who...0.....num-node-1
  set shape "circle"
  setxy random-pxcor random-pycor
  set color magenta
  ]

create-nodes 1[;who...0.....num-node-1
  set shape "circle"
  setxy random-pxcor random-pycor
  set color magenta
  ]

create-nodes 1[;who...0.....num-node-1
  set shape "circle"
  setxy random-pxcor random-pycor
  set color green
  ]

create-nodes 1[;who...0.....num-node-1
  set shape "circle"
  setxy random-pxcor random-pycor
  set color green
  ]

create-nodes 1[;who...0.....num-node-1
  set shape "circle"
  setxy random-pxcor random-pycor
  set color lime
  ]

create-nodes 1[;who...0.....num-node-1
  set shape "circle"
  setxy random-pxcor random-pycor
  set color lime
  ]

create-nodes 1[;who...0.....num-node-1
  set shape "circle"
  setxy random-pxcor random-pycor
  set color lime
  ]

create-nodes 1[;who...0.....num-node-1
  set shape "circle"
  setxy random-pxcor random-pycor
  set color lime
  ]

create-nodes 1[;who...0.....num-node-1
  set shape "circle"
  setxy random-pxcor random-pycor
  set color lime
  ]

create-nodes 1[;who...0.....num-node-1
  set shape "circle"
  setxy random-pxcor random-pycor
  set color lime
  ]

create-nodes 1[;who...0.....num-node-1
  set shape "circle"
  setxy random-pxcor random-pycor
  set color orange
  ]

create-nodes 1[;who...0.....num-node-1
  set shape "circle"
  setxy random-pxcor random-pycor
  set color orange
  ]

create-nodes 1[;who...0.....num-node-1
  set shape "circle"
  setxy random-pxcor random-pycor
  set color orange
  ]

create-nodes 1[;who...0.....num-node-1
  set shape "circle"
  setxy random-pxcor random-pycor
  set color cyan
  ]

create-nodes 1[;who...0.....num-node-1
  set shape "circle"
  setxy random-pxcor random-pycor
  set color cyan
  ]

create-nodes 1[;who...0.....num-node-1
  set shape "circle"
  setxy random-pxcor random-pycor
  set color cyan
  ]

create-nodes 1[;who...0.....num-node-1
  set shape "circle"
  setxy random-pxcor random-pycor
  set color cyan
  ]

create-nodes 1[;who...0.....num-node-1
  set shape "circle"
  setxy random-pxcor random-pycor
  set color cyan
  ]

create-nodes 1[;who...0.....num-node-1
  set shape "circle"
  setxy random-pxcor random-pycor
  set color cyan
  ]

create-nodes 1[;who...0.....num-node-1
  set shape "circle"
  setxy random-pxcor random-pycor
  set color violet
  ]

create-nodes 1[;who...0.....num-node-1
  set shape "circle"
  setxy random-pxcor random-pycor
  set color violet
  ]

create-nodes 1[;who...0.....num-node-1
  set shape "circle"
  setxy random-pxcor random-pycor
  set color violet
  ]

create-nodes 1[;who...0.....num-node-1
  set shape "circle"
  setxy random-pxcor random-pycor
  set color violet
  ]

create-nodes 1[;who...0.....num-node-1
  set shape "circle"
  setxy random-pxcor random-pycor
  set color violet
  ]

create-nodes 1[;who...0.....num-node-1
  set shape "circle"
  setxy random-pxcor random-pycor
  set color violet
  ]

create-nodes 1[;who...0.....num-node-1
  set shape "circle"
  setxy random-pxcor random-pycor
  set color violet
  ]

  ask node 0 [ create-link-to node 2  ]
  ask node 0 [ create-link-to node 3  ]
  ask node 0 [ create-link-to node 9  ]
  ask node 0 [ create-link-to node 10  ]
  ask node 0 [ create-link-to node 15  ]
  ask node 0 [ create-link-to node 16  ]
  ask node 0 [ create-link-to node 17  ]
  ask node 0 [ create-link-to node 18  ]
  ask node 0 [ create-link-to node 19  ]
  ask node 0 [ create-link-to node 21  ]
  ask node 0 [ create-link-to node 22  ]
  ask node 0 [ create-link-to node 23  ]

  ask node 1 [ create-link-to node 0  ]
  ask node 1 [ create-link-to node 3  ]
  ask node 1 [ create-link-to node 11  ]

  ask node 2 [ create-link-to node 3 ]

  ask node 3 [ create-link-to node 2  ]
  ask node 3 [ create-link-to node 6  ]
  ask node 3 [ create-link-to node 9  ]
  ask node 3 [ create-link-to node 10  ]
  ask node 3 [ create-link-to node 12  ]
  ask node 3 [ create-link-to node 15  ]
  ask node 3 [ create-link-to node 16  ]
  ask node 3 [ create-link-to node 17  ]
  ask node 3 [ create-link-to node 18  ]
  ask node 3 [ create-link-to node 21  ]
  ask node 3 [ create-link-to node 22  ]
  ask node 3 [ create-link-to node 23  ]
  ask node 3 [ create-link-to node 24  ]

  ask node 4 [ create-link-to node 3  ]
  ask node 4 [ create-link-to node 5  ]
  ask node 4 [ create-link-to node 6  ]
  ask node 4 [ create-link-to node 9  ]
  ask node 4 [ create-link-to node 15  ]
  ask node 4 [ create-link-to node 16  ]
  ask node 4 [ create-link-to node 17  ]
  ask node 4 [ create-link-to node 18  ]
  ask node 4 [ create-link-to node 21  ]
  ask node 4 [ create-link-to node 22  ]
  ask node 4 [ create-link-to node 23  ]
  ask node 4 [ create-link-to node 24  ]

  ask node 5 [ create-link-to node 3  ]
  ask node 5 [ create-link-to node 9  ]
  ask node 5 [ create-link-to node 10  ]
  ask node 5 [ create-link-to node 15  ]
  ask node 5 [ create-link-to node 16  ]
  ask node 5 [ create-link-to node 17  ]
  ask node 5 [ create-link-to node 18  ]
  ask node 5 [ create-link-to node 21  ]
  ask node 5 [ create-link-to node 22  ]
  ask node 5 [ create-link-to node 23  ]
  ask node 5 [ create-link-to node 24  ]

  ask node 6 [ create-link-to node 4  ]
  ask node 6 [ create-link-to node 5  ]
  ask node 6 [ create-link-to node 7  ]
  ask node 6 [ create-link-to node 9  ]
  ask node 6 [ create-link-to node 10  ]

  ask node 7 [ create-link-to node 3  ]
  ask node 7 [ create-link-to node 5  ]
  ask node 7 [ create-link-to node 6  ]
  ask node 7 [ create-link-to node 9  ]
  ask node 7 [ create-link-to node 15  ]
  ask node 7 [ create-link-to node 16  ]
  ask node 7 [ create-link-to node 17  ]
  ask node 7 [ create-link-to node 18  ]
  ask node 7 [ create-link-to node 21  ]
  ask node 7 [ create-link-to node 22  ]
  ask node 7 [ create-link-to node 23  ]
  ask node 7 [ create-link-to node 24  ]

  ask node 8 [ create-link-to node 7  ]
  ask node 8 [ create-link-to node 11  ]
  ask node 8 [ create-link-to node 15  ]
  ask node 8 [ create-link-to node 21  ]

  ask node 9 [ create-link-to node 3  ]
  ask node 9 [ create-link-to node 4  ]
  ask node 9 [ create-link-to node 5  ]
  ask node 9 [ create-link-to node 7  ]
  ask node 9 [ create-link-to node 8  ]
  ask node 9 [ create-link-to node 11  ]
  ask node 9 [ create-link-to node 12  ]
  ask node 9 [ create-link-to node 15  ]
  ask node 9 [ create-link-to node 16  ]
  ask node 9 [ create-link-to node 18  ]
  ask node 9 [ create-link-to node 21  ]
  ask node 9 [ create-link-to node 22  ]
  ask node 9 [ create-link-to node 23  ]
  ask node 9 [ create-link-to node 24  ]

  ask node 10 [ create-link-to node 11  ]
  ask node 10 [ create-link-to node 13  ]

  ask node 11 [ create-link-to node 4  ]
  ask node 11 [ create-link-to node 5  ]
  ask node 11 [ create-link-to node 7  ]
  ask node 11 [ create-link-to node 8  ]
  ask node 11 [ create-link-to node 13  ]
  ask node 11 [ create-link-to node 16  ]
  ask node 11 [ create-link-to node 19  ]
  ask node 11 [ create-link-to node 22  ]

  ask node 12 [ create-link-to node 10  ]

  ask node 13 [ create-link-to node 9  ]
  ask node 13 [ create-link-to node 10  ]
  ask node 13 [ create-link-to node 11  ]
  ask node 13 [ create-link-to node 12  ]
  ask node 13 [ create-link-to node 15  ]
  ask node 13 [ create-link-to node 16  ]

  ask node 14 [ create-link-to node 3  ]
  ask node 14 [ create-link-to node 4  ]
  ask node 14 [ create-link-to node 5  ]
  ask node 14 [ create-link-to node 7  ]
  ask node 14 [ create-link-to node 11  ]
  ask node 14 [ create-link-to node 15  ]
  ask node 14 [ create-link-to node 16  ]
  ask node 14 [ create-link-to node 17  ]

  ask node 15 [ create-link-to node 3  ]
  ask node 15 [ create-link-to node 4  ]
  ask node 15 [ create-link-to node 5  ]
  ask node 15 [ create-link-to node 7  ]
  ask node 15 [ create-link-to node 8  ]
  ask node 15 [ create-link-to node 9  ]
  ask node 15 [ create-link-to node 11  ]
  ask node 15 [ create-link-to node 17  ]
  ask node 15 [ create-link-to node 18  ]

  ask node 16 [ create-link-to node 11  ]

  ask node 17 [ create-link-to node 9  ]
  ask node 17 [ create-link-to node 12  ]
  ask node 17 [ create-link-to node 15  ]

  ask node 18 [ create-link-to node 3  ]
  ask node 18 [ create-link-to node 11  ]
  ask node 18 [ create-link-to node 13  ]
  ask node 18 [ create-link-to node 17  ]

  ask node 19 [ create-link-to node 10  ]
  ask node 19 [ create-link-to node 11  ]
  ask node 19 [ create-link-to node 12  ]
  ask node 19 [ create-link-to node 13  ]
  ask node 19 [ create-link-to node 21  ]
  ask node 19 [ create-link-to node 22  ]

  ask node 20 [ create-link-to node 3  ]
  ask node 20 [ create-link-to node 4  ]
  ask node 20 [ create-link-to node 5  ]
  ask node 20 [ create-link-to node 7  ]
  ask node 20 [ create-link-to node 9  ]
  ask node 20 [ create-link-to node 11  ]
  ask node 20 [ create-link-to node 14  ]
  ask node 20 [ create-link-to node 22  ]
  ask node 20 [ create-link-to node 23  ]

  ask node 21 [ create-link-to node 3  ]
  ask node 21 [ create-link-to node 4  ]
  ask node 21 [ create-link-to node 5  ]
  ask node 21 [ create-link-to node 7  ]
  ask node 21 [ create-link-to node 8  ]
  ask node 21 [ create-link-to node 9  ]
  ask node 21 [ create-link-to node 11  ]
  ask node 21 [ create-link-to node 15  ]
  ask node 21 [ create-link-to node 23  ]
  ask node 21 [ create-link-to node 24  ]

  ask node 22 [ create-link-to node 11  ]
  ask node 22 [ create-link-to node 16  ]

  ask node 23 [ create-link-to node 10  ]
  ask node 23 [ create-link-to node 12  ]
  ask node 23 [ create-link-to node 17  ]
  ask node 23 [ create-link-to node 21  ]

  ask node 24 [ create-link-to node 3  ]
  ask node 24 [ create-link-to node 10  ]
  ask node 24 [ create-link-to node 11  ]
  ask node 24 [ create-link-to node 18  ]
  ask node 24 [ create-link-to node 19  ]
  ask node 24 [ create-link-to node 23  ]

  ask node 25 [ create-link-to node 10  ]
  ask node 25 [ create-link-to node 16  ]
  ask node 25 [ create-link-to node 19  ]
  ask node 25 [ create-link-to node 24  ]



find-all-components
color-giant-component

 nw:set-context (nodes with [color = red] ) (links)

  ask node 0 [ set short_aa nw:distance-to node 0 ]
  ask node 0 [ set short_ab nw:distance-to node 1 ]
  ask node 0 [ set short_ac nw:distance-to node 2 ]
  ask node 0 [ set short_ad nw:distance-to node 3 ]
  ask node 0 [ set short_ae nw:distance-to node 4 ]
  ask node 0 [ set short_af nw:distance-to node 5 ]
  ask node 0 [ set short_ag nw:distance-to node 6 ]
  ask node 0 [ set short_ah nw:distance-to node 7 ]
  ask node 0 [ set short_ai nw:distance-to node 8 ]
  ask node 0 [ set short_aj nw:distance-to node 9 ]
  ask node 0 [ set short_ak nw:distance-to node 10 ]
  ask node 0 [ set short_al nw:distance-to node 11 ]
  ask node 0 [ set short_am nw:distance-to node 12 ]
  ask node 0 [ set short_an nw:distance-to node 13 ]
  ask node 0 [ set short_ao nw:distance-to node 14 ]
  ask node 0 [ set short_ap nw:distance-to node 15 ]
  ask node 0 [ set short_aq nw:distance-to node 16 ]
  ask node 0 [ set short_ar nw:distance-to node 17 ]
  ask node 0 [ set short_as nw:distance-to node 18 ]
  ask node 0 [ set short_at nw:distance-to node 19 ]
  ask node 0 [ set short_au nw:distance-to node 20 ]
  ask node 0 [ set short_av nw:distance-to node 21 ]
  ask node 0 [ set short_aw nw:distance-to node 22 ]
  ask node 0 [ set short_ax nw:distance-to node 23 ]
  ask node 0 [ set short_ay nw:distance-to node 24 ]
  ask node 0 [ set short_az nw:distance-to node 25 ]

  ask node 1 [ set short_ba nw:distance-to node 0 ]
  ask node 1 [ set short_bb nw:distance-to node 1 ]
  ask node 1 [ set short_bc nw:distance-to node 2 ]
  ask node 1 [ set short_bd nw:distance-to node 3 ]
  ask node 1 [ set short_be nw:distance-to node 4 ]
  ask node 1 [ set short_bf nw:distance-to node 5 ]
  ask node 1 [ set short_bg nw:distance-to node 6 ]
  ask node 1 [ set short_bh nw:distance-to node 7 ]
  ask node 1 [ set short_bi nw:distance-to node 8 ]
  ask node 1 [ set short_bj nw:distance-to node 9 ]
  ask node 1 [ set short_bk nw:distance-to node 10 ]
  ask node 1 [ set short_bl nw:distance-to node 11 ]
  ask node 1 [ set short_bm nw:distance-to node 12 ]
  ask node 1 [ set short_bn nw:distance-to node 13 ]
  ask node 1 [ set short_bo nw:distance-to node 14 ]
  ask node 1 [ set short_bp nw:distance-to node 15 ]
  ask node 1 [ set short_bq nw:distance-to node 16 ]
  ask node 1 [ set short_br nw:distance-to node 17 ]
  ask node 1 [ set short_bs nw:distance-to node 18 ]
  ask node 1 [ set short_bt nw:distance-to node 19 ]
  ask node 1 [ set short_bu nw:distance-to node 20 ]
  ask node 1 [ set short_bv nw:distance-to node 21 ]
  ask node 1 [ set short_bw nw:distance-to node 22 ]
  ask node 1 [ set short_bx nw:distance-to node 23 ]
  ask node 1 [ set short_by nw:distance-to node 24 ]
  ask node 1 [ set short_bz nw:distance-to node 25 ]


  ask nodes [ set shortc nw:distance-to node 2 ]
  ask nodes [ set shortd nw:distance-to node 3 ]
  ask nodes [ set shorte nw:distance-to node 4 ]
  ask nodes [ set shortf nw:distance-to node 5 ]
  ask nodes [ set shortg nw:distance-to node 6 ]
  ask nodes [ set shorth nw:distance-to node 7 ]
  ask nodes [ set shorti nw:distance-to node 8 ]
  ask nodes [ set shortj nw:distance-to node 9 ]
  ask nodes [ set shortk nw:distance-to node 10 ]
  ask nodes [ set shortl nw:distance-to node 11 ]
  ask nodes [ set shortm nw:distance-to node 12 ]
  ask nodes [ set shortn nw:distance-to node 13 ]

  ask node 14 [ set short_oa nw:distance-to node 0 ]
  ask node 14 [ set short_ob nw:distance-to node 1 ]
  ask node 14 [ set short_oc nw:distance-to node 2 ]
  ask node 14 [ set short_od nw:distance-to node 3 ]
  ask node 14 [ set short_oe nw:distance-to node 4 ]
  ask node 14 [ set short_of nw:distance-to node 5 ]
  ask node 14 [ set short_og nw:distance-to node 6 ]
  ask node 14 [ set short_oh nw:distance-to node 7 ]
  ask node 14 [ set short_oi nw:distance-to node 8 ]
  ask node 14 [ set short_oj nw:distance-to node 9 ]
  ask node 14 [ set short_ok nw:distance-to node 10 ]
  ask node 14 [ set short_ol nw:distance-to node 11 ]
  ask node 14 [ set short_om nw:distance-to node 12 ]
  ask node 14 [ set short_on nw:distance-to node 13 ]
  ask node 14 [ set short_oo nw:distance-to node 14 ]
  ask node 14 [ set short_op nw:distance-to node 15 ]
  ask node 14 [ set short_oq nw:distance-to node 16 ]
  ask node 14 [ set short_or nw:distance-to node 17 ]
  ask node 14 [ set short_os nw:distance-to node 18 ]
  ask node 14 [ set short_ot nw:distance-to node 19 ]
  ask node 14 [ set short_ou nw:distance-to node 20 ]
  ask node 14 [ set short_ov nw:distance-to node 21 ]
  ask node 14 [ set short_ow nw:distance-to node 22 ]
  ask node 14 [ set short_ox nw:distance-to node 23 ]
  ask node 14 [ set short_oy nw:distance-to node 24 ]
  ask node 14 [ set short_oz nw:distance-to node 25 ]

  ask nodes [ set shortp nw:distance-to node 15 ]
  ask nodes [ set shortq nw:distance-to node 16 ]
  ask nodes [ set shortr nw:distance-to node 17 ]
  ask nodes [ set shorts nw:distance-to node 18 ]
  ask nodes [ set shortt nw:distance-to node 19 ]

  ask node 20 [ set short_ua nw:distance-to node 0 ]
  ask node 20 [ set short_ub nw:distance-to node 1 ]
  ask node 20 [ set short_uc nw:distance-to node 2 ]
  ask node 20 [ set short_ud nw:distance-to node 3 ]
  ask node 20 [ set short_ue nw:distance-to node 4 ]
  ask node 20 [ set short_uf nw:distance-to node 5 ]
  ask node 20 [ set short_ug nw:distance-to node 6 ]
  ask node 20 [ set short_uh nw:distance-to node 7 ]
  ask node 20 [ set short_ui nw:distance-to node 8 ]
  ask node 20 [ set short_uj nw:distance-to node 9 ]
  ask node 20 [ set short_uk nw:distance-to node 10 ]
  ask node 20 [ set short_ul nw:distance-to node 11 ]
  ask node 20 [ set short_um nw:distance-to node 12 ]
  ask node 20 [ set short_un nw:distance-to node 13 ]
  ask node 20 [ set short_uo nw:distance-to node 14 ]
  ask node 20 [ set short_up nw:distance-to node 15 ]
  ask node 20 [ set short_uq nw:distance-to node 16 ]
  ask node 20 [ set short_ur nw:distance-to node 17 ]
  ask node 20 [ set short_us nw:distance-to node 18 ]
  ask node 20 [ set short_ut nw:distance-to node 19 ]
  ask node 20 [ set short_uu nw:distance-to node 20 ]
  ask node 20 [ set short_uv nw:distance-to node 21 ]
  ask node 20 [ set short_uw nw:distance-to node 22 ]
  ask node 20 [ set short_ux nw:distance-to node 23 ]
  ask node 20 [ set short_uy nw:distance-to node 24 ]
  ask node 20 [ set short_uz nw:distance-to node 25 ]

  ask nodes [ set shortv nw:distance-to node 21 ]
  ask nodes [ set shortw nw:distance-to node 22 ]
  ask nodes [ set shortx nw:distance-to node 23 ]
  ask nodes [ set shorty nw:distance-to node 24 ]

  ask node 25 [ set short_za nw:distance-to node 0 ]
  ask node 25 [ set short_zb nw:distance-to node 1 ]
  ask node 25 [ set short_zc nw:distance-to node 2 ]
  ask node 25 [ set short_zd nw:distance-to node 3 ]
  ask node 25 [ set short_ze nw:distance-to node 4 ]
  ask node 25 [ set short_zf nw:distance-to node 5 ]
  ask node 25 [ set short_zg nw:distance-to node 6 ]
  ask node 25 [ set short_zh nw:distance-to node 7 ]
  ask node 25 [ set short_zi nw:distance-to node 8 ]
  ask node 25 [ set short_zj nw:distance-to node 9 ]
  ask node 25 [ set short_zk nw:distance-to node 10 ]
  ask node 25 [ set short_zl nw:distance-to node 11 ]
  ask node 25 [ set short_zm nw:distance-to node 12 ]
  ask node 25 [ set short_zn nw:distance-to node 13 ]
  ask node 25 [ set short_zo nw:distance-to node 14 ]
  ask node 25 [ set short_zp nw:distance-to node 15 ]
  ask node 25 [ set short_zq nw:distance-to node 16 ]
  ask node 25 [ set short_zr nw:distance-to node 17 ]
  ask node 25 [ set short_zs nw:distance-to node 18 ]
  ask node 25 [ set short_zt nw:distance-to node 19 ]
  ask node 25 [ set short_zu nw:distance-to node 20 ]
  ask node 25 [ set short_zv nw:distance-to node 21 ]
  ask node 25 [ set short_zw nw:distance-to node 22 ]
  ask node 25 [ set short_zx nw:distance-to node 23 ]
  ask node 25 [ set short_zy nw:distance-to node 24 ]
  ask node 25 [ set short_zz nw:distance-to node 25 ]

;; Characteristic pathlength of node 0 with other nodes ;;


 ask node 0 [ set path0 0 ]
    ask node 0 [
    ifelse (short_aa = false) [
      set short_aa 0
    ]
    [
      set short_aa short_aa
     ]
  ]

      ask node 0 [
    ifelse (short_ab = false) [
      set short_ab 0
    ]
    [
      set short_ab short_ab
      set path0 path0 + 1
    ]
  ]

      ask node 0 [
    ifelse (short_ac = false) [
      set short_ac 0
    ]
    [
      set short_ac short_ac
      set path0 path0 + 1
    ]
  ]

  ask node 0 [
    ifelse (short_ad = false) [
      set short_ad 0
    ]
    [
      set short_ad short_ad
      set path0 path0 + 1
    ]
  ]

  ask node 0 [
    ifelse (short_ae = false) [
      set short_ae 0
    ]
    [
      set short_ae short_ae
      set path0 path0 + 1
    ]
  ]

  ask node 0 [
    ifelse (short_af = false) [
      set short_af 0
    ]
    [
      set short_af short_af
      set path0 path0 + 1
    ]
  ]

  ask node 0 [
    ifelse (short_ag = false) [
      set short_ag 0
    ]
    [
      set short_ag short_ag
      set path0 path0 + 1
    ]
  ]

  ask node 0 [
    ifelse (short_ah = false) [
      set short_ah 0
    ]
    [
      set short_ah short_ah
      set path0 path0 + 1
    ]
  ]

  ask node 0 [
    ifelse (short_ai = false) [
      set short_ai 0
    ]
    [
      set short_ai short_ai
      set path0 path0 + 1
    ]
  ]

  ask node 0 [
    ifelse (short_aj = false) [
      set short_aj 0
    ]
    [
      set short_aj short_aj
      set path0 path0 + 1
    ]
  ]

  ask node 0 [
    ifelse (short_ak = false) [
      set short_ak 0
    ]
    [
      set short_ak short_ak
      set path0 path0 + 1
    ]
  ]

  ask node 0 [
    ifelse (short_al = false) [
      set short_al 0
    ]
    [
      set short_al short_al
      set path0 path0 + 1
    ]
  ]

  ask node 0 [
    ifelse (short_am = false) [
      set short_am 0
    ]
    [
      set short_am short_am
      set path0 path0 + 1
    ]
  ]

  ask node 0 [
    ifelse (short_an = false) [
      set short_an 0
    ]
    [
      set short_an short_an
      set path0 path0 + 1
    ]
  ]

  ask node 0 [
    ifelse (short_ao = false) [
      set short_ao 0
    ]
    [
      set short_ao short_ao
      set path0 path0 + 1
    ]
  ]

  ask node 0 [
    ifelse (short_ap = false) [
      set short_ap 0
    ]
    [
      set short_ap short_ap
      set path0 path0 + 1
    ]
  ]

  ask node 0 [
    ifelse (short_aq = false) [
      set short_aq 0
    ]
    [
      set short_aq short_aq
      set path0 path0 + 1
    ]
  ]

  ask node 0 [
    ifelse (short_ar = false) [
      set short_ar 0
    ]
    [
      set short_ar short_ar
      set path0 path0 + 1
    ]
  ]

  ask node 0 [
    ifelse (short_as = false) [
      set short_as 0
    ]
    [
      set short_as short_as
      set path0 path0 + 1
    ]
  ]

  ask node 0 [
    ifelse (short_at = false) [
      set short_at 0
    ]
    [
      set short_at short_at
      set path0 path0 + 1
    ]
  ]

  ask node 0 [
    ifelse (short_au = false) [
      set short_au 0
    ]
    [
      set short_au short_au
      set path0 path0 + 1
    ]
  ]

  ask node 0 [
    ifelse (short_av = false) [
      set short_av 0
    ]
    [
      set short_av short_av
      set path0 path0 + 1
    ]
  ]

  ask node 0 [
    ifelse (short_aw = false) [
      set short_aw 0
    ]
    [
      set short_aw short_aw
      set path0 path0 + 1
    ]
  ]

  ask node 0 [
    ifelse (short_ax = false) [
      set short_ax 0
    ]
    [
      set short_ax short_ax
      set path0 path0 + 1
    ]
  ]

  ask node 0 [
    ifelse (short_ay = false) [
      set short_ay 0
    ]
    [
      set short_ay short_ay
      set path0 path0 + 1
    ]
  ]

  ask node 0 [
    ifelse (short_az = false) [
      set short_az 0
    ]
    [
      set short_az short_az
      set path0 path0 + 1
    ]
  ]

 ; ask node 0 [ show path0 ]

; print "Characteristic pathlength of node 0 with other nodes"
;  ask node 0 [ show short_aa ]
;  ask node 0 [ show short_ab ]
;  ask node 0 [ show short_ac ]
;  ask node 0 [ show short_ad ]
;  ask node 0 [ show short_ae ]
;  ask node 0 [ show short_af ]
;  ask node 0 [ show short_ag ]
;  ask node 0 [ show short_ah ]
;  ask node 0 [ show short_ai ]
;  ask node 0 [ show short_aj ]
;  ask node 0 [ show short_ak ]
;  ask node 0 [ show short_al ]
;  ask node 0 [ show short_am ]
;  ask node 0 [ show short_an ]
;  ask node 0 [ show short_ao ]
;  ask node 0 [ show short_ap ]
;  ask node 0 [ show short_aq ]
;  ask node 0 [ show short_ar ]
;  ask node 0 [ show short_as ]
;  ask node 0 [ show short_at ]
;  ask node 0 [ show short_au ]
;  ask node 0 [ show short_av ]
;  ask node 0 [ show short_aw ]
;  ask node 0 [ show short_ax ]
;  ask node 0 [ show short_ay ]
;  ask node 0 [ show short_az ]

  ;; Characteristic pathlength of node 1 with other nodes ;;
  ask node 1 [ set path1 0 ]
    ask node 1 [
    ifelse (short_ba = false) [
      set short_ba 0
    ]
    [
      set short_ba short_ba
      set path1 path1 + 1
    ]
  ]

      ask node 1 [
    ifelse (short_bb = false) [
      set short_bb 0
    ]
    [
      set short_bb short_bb
    ]
  ]

      ask node 1 [
    ifelse (short_bc = false) [
      set short_bc 0
    ]
    [
      set short_bc short_bc
      set path1 path1 + 1
    ]
  ]

  ask node 1 [
    ifelse (short_bd = false) [
      set short_bd 0
    ]
    [
      set short_bd short_bd
      set path1 path1 + 1
    ]
  ]

  ask node 1 [
    ifelse (short_be = false) [
      set short_be 0
    ]
    [
      set short_be short_be
      set path1 path1 + 1
    ]
  ]

  ask node 1 [
    ifelse (short_bf = false) [
      set short_bf 0
    ]
    [
      set short_bf short_bf
      set path1 path1 + 1
    ]
  ]

  ask node 1 [
    ifelse (short_bg = false) [
      set short_bg 0
    ]
    [
      set short_bg short_bg
      set path1 path1 + 1
    ]
  ]

  ask node 1 [
    ifelse (short_bh = false) [
      set short_bh 0
    ]
    [
      set short_bh short_bh
      set path1 path1 + 1
    ]
  ]

  ask node 1 [
    ifelse (short_bi = false) [
      set short_bi 0
    ]
    [
      set short_bi short_bi
      set path1 path1 + 1
    ]
  ]

  ask node 1 [
    ifelse (short_bj = false) [
      set short_bj 0
    ]
    [
      set short_bj short_bj
      set path1 path1 + 1
    ]
  ]

  ask node 1 [
    ifelse (short_bk = false) [
      set short_bk 0
    ]
    [
      set short_bk short_bk
      set path1 path1 + 1
    ]
  ]

  ask node 1 [
    ifelse (short_bl = false) [
      set short_bl 0
    ]
    [
      set short_bl short_bl
      set path1 path1 + 1
    ]
  ]

  ask node 1 [
    ifelse (short_bm = false) [
      set short_bm 0
    ]
    [
      set short_bm short_bm
      set path1 path1 + 1
    ]
  ]

  ask node 1 [
    ifelse (short_bn = false) [
      set short_bn 0
    ]
    [
      set short_bn short_bn
      set path1 path1 + 1
    ]
  ]

  ask node 1 [
    ifelse (short_bo = false) [
      set short_bo 0
    ]
    [
      set short_bo short_bo
      set path1 path1 + 1
    ]
  ]

  ask node 1 [
    ifelse (short_bp = false) [
      set short_bp 0
    ]
    [
      set short_bp short_bp
      set path1 path1 + 1
    ]
  ]

  ask node 1 [
    ifelse (short_bq = false) [
      set short_bq 0
    ]
    [
      set short_bq short_bq
      set path1 path1 + 1
    ]
  ]

  ask node 1 [
    ifelse (short_br = false) [
      set short_br 0
    ]
    [
      set short_br short_br
      set path1 path1 + 1
    ]
  ]

  ask node 1 [
    ifelse (short_bs = false) [
      set short_bs 0
    ]
    [
      set short_bs short_bs
      set path1 path1 + 1
    ]
  ]

  ask node 1 [
    ifelse (short_bt = false) [
      set short_bt 0
    ]
    [
      set short_bt short_bt
      set path1 path1 + 1
    ]
  ]

  ask node 1 [
    ifelse (short_bu = false) [
      set short_bu 0
    ]
    [
      set short_bu short_bu
      set path1 path1 + 1
    ]
  ]

  ask node 1 [
    ifelse (short_bv = false) [
      set short_bv 0
    ]
    [
      set short_bv short_bv
      set path1 path1 + 1
    ]
  ]

  ask node 1 [
    ifelse (short_bw = false) [
      set short_bw 0
    ]
    [
      set short_bw short_bw
      set path1 path1 + 1
    ]
  ]

  ask node 1 [
    ifelse (short_bx = false) [
      set short_bx 0
    ]
    [
      set short_bx short_bx
      set path1 path1 + 1
    ]
  ]

  ask node 1 [
    ifelse (short_by = false) [
      set short_by 0
    ]
    [
      set short_by short_by
      set path1 path1 + 1
    ]
  ]

  ask node 1 [
    ifelse (short_bz = false) [
      set short_bz 0
    ]
    [
      set short_bz short_bz
      set path1 path1 + 1
    ]
  ]

 ; ask node 1 [ show path1 ]

;  print "Characteristic pathlength of node 1 with other nodes"
;  ask node 1 [ show short_ba ]
;  ask node 1 [ show short_bb ]
;  ask node 1 [ show short_bc ]
;  ask node 1 [ show short_bd ]
;  ask node 1 [ show short_be ]
;  ask node 1 [ show short_bf ]
;  ask node 1 [ show short_bg ]
;  ask node 1 [ show short_bh ]
;  ask node 1 [ show short_bi ]
;  ask node 1 [ show short_bj ]
;  ask node 1 [ show short_bk ]
;  ask node 1 [ show short_bl ]
;  ask node 1 [ show short_bm ]
;  ask node 1 [ show short_bn ]
;  ask node 1 [ show short_bo ]
;  ask node 1 [ show short_bp ]
;  ask node 1 [ show short_bq ]
;  ask node 1 [ show short_br ]
;  ask node 1 [ show short_bs ]
;  ask node 1 [ show short_bt ]
;  ask node 1 [ show short_bu ]
;  ask node 1 [ show short_bv ]
;  ask node 1 [ show short_bw ]
;  ask node 1 [ show short_bx ]
;  ask node 1 [ show short_by ]
;  ask node 1 [ show short_bz ]

; print "Characteristic pathlength of node 2 with other nodes"
;  ask nodes [show short2]
;
;  print "Characteristic pathlength of node 3 with other nodes"
;  ask nodes [show short3]
;
;  print "Characteristic pathlength of node 4 with other nodes"
;  ask nodes [show short4]
;
;  print "Characteristic pathlength of node 5 with other nodes"
;  ask nodes [show short5]
;
;  print "Characteristic pathlength of node 6 with other nodes"
;  ask nodes [show short6]
;
;  print "Characteristic pathlength of node 7 with other nodes"
;  ask nodes [show short7]
;
;  print "Characteristic pathlength of node 8 with other nodes"
;  ask nodes [show short8]
;
;  print "Characteristic pathlength of node 9 with other nodes"
;  ask nodes [show short9]
;
;  print "Characteristic pathlength of node 10 with other nodes"
;  ask nodes [show short10]
;
;  print "Characteristic pathlength of node 11 with other nodes"
;  ask nodes [show short11]
;
;  print "Characteristic pathlength of node 12 with other nodes"
;  ask nodes [show short12]
;
;  print "Characteristic pathlength of node 13 with other nodes"
;  ask nodes [show short13]

   ask node 2 [

    set j 0
    set path2 0
    loop [ ifelse (j = 26)

      [ stop ]
    [
      if (nw:distance-to node j != 0) [
      set path2 path2 + 1
    ]

  ]
      set j j + 1
    ]
  ]
 ; ask node 2 [ show path2 ]


ask node 3 [

    set j 0
    set path3 0
    loop [ ifelse (j = 26)

      [ stop ]
    [
      if (nw:distance-to node j != 0) [
      set path3 path3 + 1
    ]

  ]
      set j j + 1
    ]
  ]
 ; ask node 3 [ show path3 ]


ask node 4 [

    set j 0
    set path4 0
    loop [ ifelse (j = 26)

      [ stop ]
    [
      if (nw:distance-to node j != 0) [
      set path4 path4 + 1
    ]

  ]
      set j j + 1
    ]
  ]
 ; ask node 4 [ show path4 ]


ask node 5 [

    set j 0
    set path5 0
    loop [ ifelse (j = 26)

      [ stop ]
    [
      if (nw:distance-to node j != 0) [
      set path5 path5 + 1
    ]

  ]
      set j j + 1
    ]
  ]
;  ask node 5 [ show path5 ]

  ask node 6 [

    set j 0
    set path6 0
    loop [ ifelse (j = 26)

      [ stop ]
    [
      if (nw:distance-to node j != 0) [
      set path6 path6 + 1
    ]

  ]
      set j j + 1
    ]
  ]
;  ask node 6 [ show path6 ]


ask node 7 [

    set j 0
    set path7 0
    loop [ ifelse (j = 26)

      [ stop ]
    [
      if (nw:distance-to node j != 0) [
      set path7 path7 + 1
    ]

  ]
      set j j + 1
    ]
  ]
;  ask node 7 [ show path7 ]


ask node 8 [

    set j 0
    set path8 0
    loop [ ifelse (j = 26)

      [ stop ]
    [
      if (nw:distance-to node j != 0) [
      set path8 path8 + 1
    ]

  ]
      set j j + 1
    ]
  ]
 ; ask node 8 [ show path8 ]


ask node 9 [

    set j 0
    set path9 0
    loop [ ifelse (j = 26)

      [ stop ]
    [
      if (nw:distance-to node j != 0) [
      set path9 path9 + 1
    ]

  ]
      set j j + 1
    ]
  ]
;  ask node 9 [ show path9 ]


  ask node 10 [

    set j 0
    set path10 0
    loop [ ifelse (j = 26)

      [ stop ]
    [
      if (nw:distance-to node j != 0) [
      set path10 path10 + 1
    ]

  ]
      set j j + 1
    ]
  ]
 ; ask node 10 [ show path10 ]


ask node 11 [

    set j 0
    set path11 0
    loop [ ifelse (j = 26)

      [ stop ]
    [
      if (nw:distance-to node j != 0) [
      set path11 path11 + 1
    ]

  ]
      set j j + 1
    ]
  ]
 ; ask node 11 [ show path11 ]


ask node 12 [

    set j 0
    set path12 0
    loop [ ifelse (j = 26)

      [ stop ]
    [
      if (nw:distance-to node j != 0) [
      set path12 path12 + 1
    ]

  ]
      set j j + 1
    ]
  ]
 ; ask node 12 [ show path12 ]


ask node 13 [

    set j 0
    set path13 0
    loop [ ifelse (j = 26)

      [ stop ]
    [
      if (nw:distance-to node j != 0) [
      set path13 path13 + 1
    ]

  ]
      set j j + 1
    ]
  ]
;  ask node 13 [ show path13 ]

;; Characteristic pathlength of node 14 with other nodes ;;
  ask node 14 [ set path14 0 ]
 ask node 14 [
    ifelse (short_oa = false) [
      set short_oa 0
    ]
    [
      set short_oa short_oa
      set path14 path14 + 1
    ]
  ]

      ask node 14 [
    ifelse (short_ob = false) [
      set short_ob 0
    ]
    [
      set short_ob short_ob
      set path14 path14 + 1
    ]
  ]

      ask node 14 [
    ifelse (short_oc = false) [
      set short_oc 0
    ]
    [
      set short_oc short_oc
      set path14 path14 + 1
    ]
  ]

  ask node 14 [
    ifelse (short_od = false) [
      set short_od 0
    ]
    [
      set short_od short_od
      set path14 path14 + 1
    ]
  ]

  ask node 14 [
    ifelse (short_oe = false) [
      set short_oe 0
    ]
    [
      set short_oe short_oe
      set path14 path14 + 1
    ]
  ]

  ask node 14 [
    ifelse (short_of = false) [
      set short_of 0
    ]
    [
      set short_of short_of
      set path14 path14 + 1
    ]
  ]

  ask node 14 [
    ifelse (short_og = false) [
      set short_og 0
    ]
    [
      set short_og short_og
      set path14 path14 + 1
    ]
  ]

  ask node 14 [
    ifelse (short_oh = false) [
      set short_oh 0
    ]
    [
      set short_oh short_oh
      set path14 path14 + 1
    ]
  ]

  ask node 14 [
    ifelse (short_oi = false) [
      set short_oi 0
    ]
    [
      set short_oi short_oi
      set path14 path14 + 1
    ]
  ]

  ask node 14 [
    ifelse (short_oj = false) [
      set short_oj 0
    ]
    [
      set short_oj short_oj
      set path14 path14 + 1
    ]
  ]

  ask node 14 [
    ifelse (short_ok = false) [
      set short_ok 0
    ]
    [
      set short_ok short_ok
      set path14 path14 + 1
    ]
  ]

  ask node 14 [
    ifelse (short_ol = false) [
      set short_ol 0
    ]
    [
      set short_ol short_ol
      set path14 path14 + 1
    ]
  ]

  ask node 14 [
    ifelse (short_om = false) [
      set short_om 0
    ]
    [
      set short_om short_om
      set path14 path14 + 1
    ]
  ]

  ask node 14 [
    ifelse (short_on = false) [
      set short_on 0
    ]
    [
      set short_on short_on
      set path14 path14 + 1
    ]
  ]

  ask node 14 [
    ifelse (short_oo = false) [
      set short_oo 0
    ]
    [
      set short_oo short_oo
    ]
  ]

  ask node 14 [
    ifelse (short_op = false) [
      set short_op 0
    ]
    [
      set short_op short_op
      set path14 path14 + 1
    ]
  ]

  ask node 14 [
    ifelse (short_oq = false) [
      set short_oq 0
    ]
    [
      set short_oq short_oq
      set path14 path14 + 1
    ]
  ]

  ask node 14 [
    ifelse (short_or = false) [
      set short_or 0
    ]
    [
      set short_or short_or
      set path14 path14 + 1
    ]
  ]

  ask node 14 [
    ifelse (short_os = false) [
      set short_os 0
    ]
    [
      set short_os short_os
      set path14 path14 + 1
    ]
  ]

  ask node 14 [
    ifelse (short_ot = false) [
      set short_ot 0
    ]
    [
      set short_ot short_ot
      set path14 path14 + 1
    ]
  ]

  ask node 14 [
    ifelse (short_ou = false) [
      set short_ou 0
    ]
    [
      set short_ou short_ou
      set path14 path14 + 1
    ]
  ]

  ask node 14 [
    ifelse (short_ov = false) [
      set short_ov 0
    ]
    [
      set short_ov short_ov
      set path14 path14 + 1
    ]
  ]

  ask node 14 [
    ifelse (short_ow = false) [
      set short_ow 0
    ]
    [
      set short_ow short_ow
      set path14 path14 + 1
    ]
  ]

  ask node 14 [
    ifelse (short_ox = false) [
      set short_ox 0
    ]
    [
      set short_ox short_ox
      set path14 path14 + 1
    ]
  ]

  ask node 14 [
    ifelse (short_oy = false) [
      set short_oy 0
    ]
    [
      set short_oy short_oy
      set path14 path14 + 1
    ]
  ]

  ask node 14 [
    ifelse (short_oz = false) [
      set short_oz 0
    ]
    [
      set short_oz short_oz
      set path14 path14 + 1
    ]
  ]

 ; ask node 14 [ show path14 ]


;  print "Characteristic pathlength of node 14 with other nodes"
;  ask node 14 [ show short_oa ]
;  ask node 14 [ show short_ob ]
;  ask node 14 [ show short_oc ]
;  ask node 14 [ show short_od ]
;  ask node 14 [ show short_oe ]
;  ask node 14 [ show short_of ]
;  ask node 14 [ show short_og ]
;  ask node 14 [ show short_oh ]
;  ask node 14 [ show short_oi ]
;  ask node 14 [ show short_oj ]
;  ask node 14 [ show short_ok ]
;  ask node 14 [ show short_ol ]
;  ask node 14 [ show short_om ]
;  ask node 14 [ show short_on ]
;  ask node 14 [ show short_oo ]
;  ask node 14 [ show short_op ]
;  ask node 14 [ show short_oq ]
;  ask node 14 [ show short_or ]
;  ask node 14 [ show short_os ]
;  ask node 14 [ show short_ot ]
;  ask node 14 [ show short_ou ]
;  ask node 14 [ show short_ov ]
;  ask node 14 [ show short_ow ]
;  ask node 14 [ show short_ox ]
;  ask node 14 [ show short_oy ]
;  ask node 14 [ show short_oz ]

;  print "Characteristic pathlength of node 15 with other nodes"
;  ask nodes [show short15]
;
;  print "Characteristic pathlength of node 16 with other nodes"
;  ask nodes [show short16]
;
;  print "Characteristic pathlength of node 17 with other nodes"
;  ask nodes [show short17]
;
;  print "Characteristic pathlength of node 18 with other nodes"
;  ask nodes [show short18]
;
;  print "Characteristic pathlength of node 19 with other nodes"
;  ask nodes [show short19]
ask node 15 [

    set j 0
    set path15 0
    loop [ ifelse (j = 26)

      [ stop ]
    [
      if (nw:distance-to node j != 0) [
      set path15 path15 + 1
    ]

  ]
      set j j + 1
    ]
  ]
;  ask node 15 [ show path15 ]


ask node 16 [

    set j 0
    set path16 0
    loop [ ifelse (j = 26)

      [ stop ]
    [
      if (nw:distance-to node j != 0) [
      set path16 path16 + 1
    ]

  ]
      set j j + 1
    ]
  ]
 ; ask node 16 [ show path16 ]


ask node 17 [

    set j 0
    set path17 0
    loop [ ifelse (j = 26)

      [ stop ]
    [
      if (nw:distance-to node j != 0) [
      set path17 path17 + 1
    ]

  ]
      set j j + 1
    ]
  ]
;  ask node 17 [ show path17 ]

    ask node 18 [

    set j 0
    set path18 0
    loop [ ifelse (j = 26)

      [ stop ]
    [
      if (nw:distance-to node j != 0) [
      set path18 path18 + 1
    ]

  ]
      set j j + 1
    ]
  ]
 ; ask node 18 [ show path18 ]


ask node 19 [

    set j 0
    set path19 0
    loop [ ifelse (j = 26)

      [ stop ]
    [
      if (nw:distance-to node j != 0) [
      set path19 path19 + 1
    ]

  ]
      set j j + 1
    ]
  ]
;  ask node 19 [ show path19 ]

;; Characteristic pathlength of node 20 with other nodes ;;
 ask node 20 [ set path20 0 ]
 ask node 20 [
    ifelse (short_ua = false) [
      set short_ua 0
    ]
    [
      set short_ua short_ua
      set path20 path20 + 1
    ]
  ]

      ask node 20 [
    ifelse (short_ub = false) [
      set short_ub 0
    ]
    [
      set short_ub short_ub
      set path20 path20 + 1
    ]
  ]

      ask node 20 [
    ifelse (short_uc = false) [
      set short_uc 0
    ]
    [
      set short_uc short_uc
      set path20 path20 + 1
    ]
  ]

  ask node 20 [
    ifelse (short_ud = false) [
      set short_ud 0
    ]
    [
      set short_ud short_ud
      set path20 path20 + 1
    ]
  ]

  ask node 20 [
    ifelse (short_ue = false) [
      set short_ue 0
    ]
    [
      set short_ue short_ue
      set path20 path20 + 1
    ]
  ]

  ask node 20 [
    ifelse (short_uf = false) [
      set short_uf 0
    ]
    [
      set short_uf short_uf
      set path20 path20 + 1
    ]
  ]

  ask node 20 [
    ifelse (short_ug = false) [
      set short_ug 0
    ]
    [
      set short_ug short_ug
      set path20 path20 + 1
    ]
  ]

  ask node 20 [
    ifelse (short_uh = false) [
      set short_uh 0
    ]
    [
      set short_uh short_uh
      set path20 path20 + 1
    ]
  ]

  ask node 20 [
    ifelse (short_ui = false) [
      set short_ui 0
    ]
    [
      set short_ui short_ui
      set path20 path20 + 1
    ]
  ]

  ask node 20 [
    ifelse (short_uj = false) [
      set short_uj 0
    ]
    [
      set short_uj short_uj
      set path20 path20 + 1
    ]
  ]

  ask node 20 [
    ifelse (short_uk = false) [
      set short_uk 0
    ]
    [
      set short_uk short_uk
      set path20 path20 + 1
    ]
  ]

  ask node 20 [
    ifelse (short_ul = false) [
      set short_ul 0
    ]
    [
      set short_ul short_ul
      set path20 path20 + 1
    ]
  ]

  ask node 20 [
    ifelse (short_um = false) [
      set short_um 0
    ]
    [
      set short_um short_um
      set path20 path20 + 1
    ]
  ]

  ask node 20 [
    ifelse (short_un = false) [
      set short_un 0
    ]
    [
      set short_un short_un
      set path20 path20 + 1
    ]
  ]

  ask node 20 [
    ifelse (short_uo = false) [
      set short_uo 0
    ]
    [
      set short_uo short_uo
      set path20 path20 + 1
    ]
  ]

  ask node 20 [
    ifelse (short_up = false) [
      set short_up 0
    ]
    [
      set short_up short_up
      set path20 path20 + 1
    ]
  ]

  ask node 20 [
    ifelse (short_uq = false) [
      set short_uq 0
    ]
    [
      set short_uq short_uq
      set path20 path20 + 1
    ]
  ]

  ask node 20 [
    ifelse (short_ur = false) [
      set short_ur 0
    ]
    [
      set short_ur short_ur
      set path20 path20 + 1
    ]
  ]

  ask node 20 [
    ifelse (short_us = false) [
      set short_us 0
    ]
    [
      set short_us short_us
      set path20 path20 + 1
    ]
  ]

  ask node 20 [
    ifelse (short_ut = false) [
      set short_ut 0
    ]
    [
      set short_ut short_ut
      set path20 path20 + 1
    ]
  ]

  ask node 20 [
    ifelse (short_uu = false) [
      set short_uu 0
    ]
    [
      set short_uu short_uu
    ]
  ]

  ask node 20 [
    ifelse (short_uv = false) [
      set short_uv 0
    ]
    [
      set short_uv short_uv
      set path20 path20 + 1
    ]
  ]

  ask node 20 [
    ifelse (short_uw = false) [
      set short_uw 0
    ]
    [
      set short_uw short_uw
      set path20 path20 + 1
    ]
  ]

  ask node 20 [
    ifelse (short_ux = false) [
      set short_ux 0
    ]
    [
      set short_ux short_ux
      set path20 path20 + 1
    ]
  ]

  ask node 20 [
    ifelse (short_uy = false) [
      set short_uy 0
    ]
    [
      set short_uy short_uy
      set path20 path20 + 1
    ]
  ]

  ask node 20 [
    ifelse (short_uz = false) [
      set short_uz 0
    ]
    [
      set short_uz short_uz
      set path20 path20 + 1
    ]
  ]

 ; ask node 20 [ show path20 ]

;  print "Characteristic pathlength of node 20 with other nodes"
;  ask node 20 [ show short_ua ]
;  ask node 20 [ show short_ub ]
;  ask node 20 [ show short_uc ]
;  ask node 20 [ show short_ud ]
;  ask node 20 [ show short_ue ]
;  ask node 20 [ show short_uf ]
;  ask node 20 [ show short_ug ]
;  ask node 20 [ show short_uh ]
;  ask node 20 [ show short_ui ]
;  ask node 20 [ show short_uj ]
;  ask node 20 [ show short_uk ]
;  ask node 20 [ show short_ul ]
;  ask node 20 [ show short_um ]
;  ask node 20 [ show short_un ]
;  ask node 20 [ show short_uo ]
;  ask node 20 [ show short_up ]
;  ask node 20 [ show short_uq ]
;  ask node 20 [ show short_ur ]
;  ask node 20 [ show short_us ]
;  ask node 20 [ show short_ut ]
;  ask node 20 [ show short_uu ]
;  ask node 20 [ show short_uv ]
;  ask node 20 [ show short_uw ]
;  ask node 20 [ show short_ux ]
;  ask node 20 [ show short_uy ]
;  ask node 20 [ show short_uz ]
;
;  print "Characteristic pathlength of node 21 with other nodes"
;  ask nodes [show short21]
;
;  print "Characteristic pathlength of node 22 with other nodes"
;  ask nodes [show short22]
;
;  print "Characteristic pathlength of node 23 with other nodes"
;  ask nodes [show short23]
;
;  print "Characteristic pathlength of node 24 with other nodes"
;  ask nodes [show short24]

ask node 21 [

    set j 0
    set path21 0
    loop [ ifelse (j = 26)

      [ stop ]
    [
      if (nw:distance-to node j != 0) [
      set path21 path21 + 1
    ]

  ]
      set j j + 1
    ]
  ]
 ; ask node 21 [ show path21 ]


ask node 22 [

    set j 0
    set path22 0
    loop [ ifelse (j = 26)

      [ stop ]
    [
      if (nw:distance-to node j != 0) [
      set path22 path22 + 1
    ]

  ]
      set j j + 1
    ]
  ]
;  ask node 22 [ show path22 ]

  ask node 23 [

    set j 0
    set path23 0
    loop [ ifelse (j = 26)

      [ stop ]
    [
      if (nw:distance-to node j != 0) [
      set path23 path23 + 1
    ]

  ]
      set j j + 1
    ]
  ]
;  ask node 23 [ show path23 ]


ask node 24 [

    set j 0
    set path24 0
    loop [ ifelse (j = 26)

      [ stop ]
    [
      if (nw:distance-to node j != 0) [
      set path24 path24 + 1
    ]

  ]
      set j j + 1
    ]
  ]
;  ask node 24 [ show path24 ]


  ;; Characteristic pathlength of node 25 with other nodes ;;
  ask node 25 [ set path25 0 ]
  ask node 25 [
    ifelse (short_za = false) [
      set short_za 0
    ]
    [
      set short_za short_za
      set path25 path25 + 1
    ]
  ]

      ask node 25 [
    ifelse (short_zb = false) [
      set short_zb 0
    ]
    [
      set short_zb short_zb
      set path25 path25 + 1
    ]
  ]

      ask node 25 [
    ifelse (short_zc = false) [
      set short_zc 0
    ]
    [
      set short_zc short_zc
      set path25 path25 + 1
    ]
  ]

  ask node 25 [
    ifelse (short_zd = false) [
      set short_zd 0
    ]
    [
      set short_zd short_zd

    ]
  ]

  ask node 25 [
    ifelse (short_ze = false) [
      set short_ze 0
    ]
    [
      set short_ze short_ze
      set path25 path25 + 1
    ]
  ]

  ask node 25 [
    ifelse (short_zf = false) [
      set short_zf 0
    ]
    [
      set short_zf short_zf
      set path25 path25 + 1
    ]
  ]

  ask node 25 [
    ifelse (short_zg = false) [
      set short_zg 0
    ]
    [
      set short_zg short_zg
      set path25 path25 + 1
    ]
  ]

  ask node 25 [
    ifelse (short_zh = false) [
      set short_zh 0
    ]
    [
      set short_zh short_zh
      set path25 path25 + 1
    ]
  ]

  ask node 25 [
    ifelse (short_zi = false) [
      set short_zi 0
    ]
    [
      set short_zi short_zi
      set path25 path25 + 1
    ]
  ]

  ask node 25 [
    ifelse (short_zj = false) [
      set short_zj 0
    ]
    [
      set short_zj short_zj
      set path25 path25 + 1
    ]
  ]

  ask node 25 [
    ifelse (short_zk = false) [
      set short_zk 0
    ]
    [
      set short_zk short_zk
      set path25 path25 + 1
    ]
  ]

  ask node 25 [
    ifelse (short_zl = false) [
      set short_zl 0
    ]
    [
      set short_zl short_zl
      set path25 path25 + 1
    ]
  ]

  ask node 25 [
    ifelse (short_zm = false) [
      set short_zm 0
    ]
    [
      set short_zm short_zm
      set path25 path25 + 1
    ]
  ]

  ask node 25 [
    ifelse (short_zn = false) [
      set short_zn 0
    ]
    [
      set short_zn short_zn
      set path25 path25 + 1
    ]
  ]

  ask node 25 [
    ifelse (short_zo = false) [
      set short_zo 0
    ]
    [
      set short_zo short_zo
      set path25 path25 + 1
    ]
  ]

  ask node 25 [
    ifelse (short_zp = false) [
      set short_zp 0
    ]
    [
      set short_zp short_zp
      set path25 path25 + 1
    ]
  ]

  ask node 25 [
    ifelse (short_zq = false) [
      set short_zq 0
    ]
    [
      set short_zq short_zq
      set path25 path25 + 1
    ]
  ]

  ask node 25 [
    ifelse (short_zr = false) [
      set short_zr 0
    ]
    [
      set short_zr short_zr
      set path25 path25 + 1
    ]
  ]

  ask node 25 [
    ifelse (short_zs = false) [
      set short_zs 0
    ]
    [
      set short_zs short_zs
      set path25 path25 + 1
    ]
  ]

  ask node 25 [
    ifelse (short_zt = false) [
      set short_zt 0
    ]
    [
      set short_zt short_zt
      set path25 path25 + 1
    ]
  ]

  ask node 25 [
    ifelse (short_zu = false) [
      set short_zu 0
    ]
    [
      set short_zu short_zu
      set path25 path25 + 1
    ]
  ]

  ask node 25 [
    ifelse (short_zv = false) [
      set short_zv 0
    ]
    [
      set short_zv short_zv
      set path25 path25 + 1
    ]
  ]

  ask node 25 [
    ifelse (short_zw = false) [
      set short_zw 0
    ]
    [
      set short_zw short_zw
      set path25 path25 + 1
    ]
  ]

  ask node 25 [
    ifelse (short_zx = false) [
      set short_zx 0
    ]
    [
      set short_zx short_zx
      set path25 path25 + 1
    ]
  ]

  ask node 25 [
    ifelse (short_zy = false) [
      set short_zy 0
    ]
    [
      set short_zy short_zy
      set path25 path25 + 1
    ]
  ]

  ask node 25 [
    ifelse (short_zz = false) [
      set short_zz 0
    ]
    [
      set short_zz short_zz
      set path25 path25 + 1
    ]
  ]

;  ask node 25 [ show path25 ]

;  print "Characteristic pathlength of node 25 with other nodes"
;  ask node 25 [ show short_za ]
;  ask node 25 [ show short_zb ]
;  ask node 25 [ show short_zc ]
;  ask node 25 [ show short_zd ]
;  ask node 25 [ show short_ze ]
;  ask node 25 [ show short_zf ]
;  ask node 25 [ show short_zg ]
;  ask node 25 [ show short_zh ]
;  ask node 25 [ show short_zi ]
;  ask node 25 [ show short_zj ]
;  ask node 25 [ show short_zk ]
;  ask node 25 [ show short_zl ]
;  ask node 25 [ show short_zm ]
;  ask node 25 [ show short_zn ]
;  ask node 25 [ show short_zo ]
;  ask node 25 [ show short_zp ]
;  ask node 25 [ show short_zq ]
;  ask node 25 [ show short_zr ]
;  ask node 25 [ show short_zs ]
;  ask node 25 [ show short_zt ]
;  ask node 25 [ show short_zu ]
;  ask node 25 [ show short_zv ]
;  ask node 25 [ show short_zw ]
;  ask node 25 [ show short_zx ]
;  ask node 25 [ show short_zy ]
;  ask node 25 [ show short_zz ]


  ask node 0 [ set short0 short_aa + short_ab + short_ac + short_ad + short_ae + short_af + short_ag + short_ah + short_ai + short_aj + short_ak + short_al + short_am + short_an + short_ao + short_ap + short_aq + short_ar + short_as + short_at + short_au + short_av + short_aw + short_ax + short_ay + short_az ]
  ask node 1 [ set short1 short_ba + short_bb + short_bc + short_bd + short_be + short_bf + short_bg + short_bh + short_bi + short_bj + short_bk + short_bl + short_bm + short_bn + short_bo + short_bp + short_bq + short_br + short_bs + short_bt + short_bu + short_bv + short_bw + short_bx + short_by + short_bz ]
  ask node 2 [ set short2 sum[shortc] of nodes]
  ask node 3 [ set short3 sum[shortd] of nodes]
  ask node 4 [ set short4 sum[shorte] of nodes]
  ask node 5 [ set short5 sum[shortf] of nodes]
  ask node 6 [ set short6 sum[shortg] of nodes]
  ask node 7 [ set short7 sum[shorth] of nodes]
  ask node 8 [ set short8 sum[shorti] of nodes]
  ask node 9 [ set short9 sum[shortj] of nodes]
  ask node 10 [ set short10 sum[shortk] of nodes]
  ask node 11 [ set short11 sum[shortl] of nodes]
  ask node 12 [ set short12 sum[shortm] of nodes]
  ask node 13 [ set short13 sum[shortn] of nodes]
  ask node 14 [ set short14 short_oa + short_ob + short_oc + short_od + short_oe + short_of + short_og + short_oh + short_oi + short_oj + short_ok + short_ol + short_om + short_on + short_oo + short_op + short_oq + short_or + short_os + short_ot + short_ou + short_ov + short_ow + short_ox + short_oy + short_oz ]
  ask node 15 [ set short15 sum[shortp] of nodes]
  ask node 16 [ set short16 sum[shortq] of nodes]
  ask node 17 [ set short17 sum[shortr] of nodes]
  ask node 18 [ set short18 sum[shorts] of nodes]
  ask node 19 [ set short19 sum[shortt] of nodes]
  ask node 20 [ set short20 short_ua + short_ub + short_uc + short_ud + short_ue + short_uf + short_ug + short_uh + short_ui + short_uj + short_uk + short_ul + short_um + short_un + short_uo + short_up + short_uq + short_ur + short_us + short_ut + short_uu + short_uv + short_uw + short_ux + short_uy + short_uz ]
  ask node 21 [ set short21 sum[shortv] of nodes]
  ask node 22 [ set short22 sum[shortw] of nodes]
  ask node 23 [ set short23 sum[shortx] of nodes]
  ask node 24 [ set short24 sum[shorty] of nodes]
  ask node 25 [ set short25 short_za + short_zb + short_zc + short_zd + short_ze + short_zf + short_zg + short_zh + short_zi + short_zj + short_zk + short_zl + short_zm + short_zn + short_zo + short_zp + short_zq + short_zr + short_zs + short_zt + short_zu + short_zv + short_zw + short_zx + short_zy + short_zz ]

;  ask node 0 [show short0]
;  ask node 1 [show short1]
;  ask node 2 [show short2]
;  ask node 3 [show short3]
;  ask node 4 [show short4]
;  ask node 5 [show short5]
;  ask node 6 [show short6]
;  ask node 7 [show short7]
;  ask node 8 [show short8]
;  ask node 9 [show short9]
;  ask node 10 [show short10]
;  ask node 11 [show short11]
;  ask node 12 [show short12]
;  ask node 13 [show short13]
;  ask node 14 [show short14]
;  ask node 15 [show short15]
;  ask node 16 [show short16]
;  ask node 17 [show short17]
;  ask node 18 [show short18]
;  ask node 19 [show short19]
;  ask node 20 [show short20]
;  ask node 21 [show short21]
;  ask node 22 [show short22]
;  ask node 23 [show short23]
;  ask node 24 [show short24]
;  ask node 25 [show short25]
  ask nodes [ set short short0 + short1 + short2 + short3 + short4 + short5 + short6 + short7 + short8 + short9 + short10 + short11 + short12 + short13 + short14 + short15 + short16 + short17 + short18 + short19 + short20 + short21 + short22 + short23 + short24 + short25 ]
  set pathlength sum[short] of nodes
  show pathlength

    ask nodes [ set path path0 + path1 + path2 + path3 + path4 + path5 + path6 + path7 + path8 + path9 + path10 + path11 + path12 + path13 + path14 + path15 + path16 + path17 + path18 + path19 + path20 + path21 + path22 + path23 + path24 + path25 ]
  ask nodes [ show path ]
 set pathposs sum[path] of nodes
 show pathposs

;;;; Clustering coefficient ;;

  ask node 0 [ set cluster0 [nw:clustering-coefficient] of node 0 ]
  ask node 1 [ set cluster1 [nw:clustering-coefficient] of node 1 ]
  ask node 2 [ set cluster2 [nw:clustering-coefficient] of node 2 ]
  ask node 3 [ set cluster3 [nw:clustering-coefficient] of node 3 ]
  ask node 4 [ set cluster4 [nw:clustering-coefficient] of node 4 ]
  ask node 5 [ set cluster5 [nw:clustering-coefficient] of node 5 ]
  ask node 6 [ set cluster6 [nw:clustering-coefficient] of node 6 ]
  ask node 7 [ set cluster7 [nw:clustering-coefficient] of node 7 ]
  ask node 8 [ set cluster8 [nw:clustering-coefficient] of node 8 ]
  ask node 9 [ set cluster9 [nw:clustering-coefficient] of node 9 ]
  ask node 10 [ set cluster10 [nw:clustering-coefficient] of node 10 ]
  ask node 11 [ set cluster11 [nw:clustering-coefficient] of node 11 ]
  ask node 12 [ set cluster12 [nw:clustering-coefficient] of node 12 ]
  ask node 13 [ set cluster13 [nw:clustering-coefficient] of node 13 ]
  ask node 14 [ set cluster14 [nw:clustering-coefficient] of node 14 ]
  ask node 15 [ set cluster15 [nw:clustering-coefficient] of node 15 ]
  ask node 16 [ set cluster16 [nw:clustering-coefficient] of node 16 ]
  ask node 17 [ set cluster17 [nw:clustering-coefficient] of node 17 ]
  ask node 18 [ set cluster18 [nw:clustering-coefficient] of node 18 ]
  ask node 19 [ set cluster19 [nw:clustering-coefficient] of node 19 ]
  ask node 20 [ set cluster20 [nw:clustering-coefficient] of node 20 ]
  ask node 21 [ set cluster21 [nw:clustering-coefficient] of node 21 ]
  ask node 22 [ set cluster22 [nw:clustering-coefficient] of node 22 ]
  ask node 23 [ set cluster23 [nw:clustering-coefficient] of node 23 ]
  ask node 24 [ set cluster24 [nw:clustering-coefficient] of node 24 ]
  ask node 25 [ set cluster25 [nw:clustering-coefficient] of node 25 ]
  ask node 0 [ show cluster0 ]
  ask node 1 [ show cluster1 ]
  ask node 2 [ show cluster2 ]
  ask node 3 [ show cluster3 ]
  ask node 4 [ show cluster4 ]
  ask node 5 [ show cluster5 ]
  ask node 6 [ show cluster6 ]
  ask node 7 [ show cluster7 ]
  ask node 8 [ show cluster8 ]
  ask node 9 [ show cluster9 ]
  ask node 10 [ show cluster10 ]
  ask node 11 [ show cluster11 ]
  ask node 12 [ show cluster12 ]
  ask node 13 [ show cluster13 ]
  ask node 14 [ show cluster14 ]
  ask node 15 [ show cluster15 ]
  ask node 16 [ show cluster16 ]
  ask node 17 [ show cluster17 ]
  ask node 18 [ show cluster18 ]
  ask node 19 [ show cluster19 ]
  ask node 20 [ show cluster20 ]
  ask node 21 [ show cluster21 ]
  ask node 22 [ show cluster22 ]
  ask node 23 [ show cluster23 ]
  ask node 24 [ show cluster24 ]
  ask node 25 [ show cluster25 ]
  set meancluster mean [nw:clustering-coefficient] of nodes
  show meancluster


reset-ticks


end







;;;;;;;;;;;;;;;;;;;;;;
;;; Main Procedure ;;;
;;;;;;;;;;;;;;;;;;;;;;

to go-random
  ;; if the below condition is true then we have a fully disconnected network and we need to stop
  if (count links = 0) [
    display
    user-message "Network is fully disconnected. No more edges can be removed."
    stop
  ]


  remove-edge-random
  find-all-components-new
  color-giant-component
  ask links [ set color [color] of end1 ]  ;; recolor all edges
  layout-1
  tick
end





;;;;;;;;;;;;;;;;;;;;;;;
;;; Edge removals ;;;
;;;;;;;;;;;;;;;;;;;;;;;

;; pick a random node and remove its link

to remove-edge-random


    ask one-of nodes [

    ifelse (count my-links = 0) [
    remove-edge-random
    ]

    [set color red
    ask my-links [die]
            ]
    ]

end


;;;;;;;;;;;;;;;;;;;;;;;;;;;
;;; Network Exploration ;;;
;;;;;;;;;;;;;;;;;;;;;;;;;;;

;; to find all the connected components in the network, their sizes and starting turtles
to find-all-components
  ask nodes [ set explored? false ]
  ;; keep exploring till all turtles get explored
  loop
  [


    ;; pick a node that has not yet been explored
    let start one-of nodes with [ not explored? ]
    if start = nobody [ stop ]
    ;; reset the number of turtles found to 0
    ;; this variable is updated each time we explore an
    ;; unexplored node.
    set component-size 0

    ;; at this stage, we recolor everything to light gray
    ask start [ explore (gray + 2) ]
    ;; the explore procedure updates the component-size variable.
    ;; so check, have we found a new giant component?
    if component-size > giant-component-size
    [
      set giant-component-size component-size

      set giant-start-node start
    ]
  ]
end


to find-all-components-new
  ask nodes [ set explored? false ]
  set giant-component-size 0   ;;;; to start new search about the new giant components
  ;; keep exploring till all turtles get explored
  loop
  [


    ;; pick a node that has not yet been explored
    let start one-of nodes with [ not explored? ]
    if start = nobody [ stop ]
    ;; reset the number of turtles found to 0
    ;; this variable is updated each time we explore an
    ;; unexplored node.
    set component-size 0

    ;; at this stage, we recolor everything to light gray
    ask start [ explore (gray + 2) ]
    ;; the explore procedure updates the component-size variable.
    ;; so check, have we found a new giant component?
    if component-size > giant-component-size
    [
      set giant-component-size component-size

      set giant-start-node start
    ]
  ]
end



to explore [new-color]  ;; node procedure
  if explored? [ stop ]
  set explored? true
  set component-size component-size + 1
  ;; color the node
  set color new-color
  ask link-neighbors [ explore new-color ]

end



;; color the giant component red
to color-giant-component
  ask nodes [ set explored? false ]
  set component-size 0
  ask giant-start-node [ explore red ]
end


;;;;;;;;;;;;;;
;;; Layout ;;;
;;;;;;;;;;;;;;


to layout
  layout-spring nodes links 0.2 5 0.2

end


to layout-1
  ;if not layout-1? [ stop ]
  ;; the number 10 here is arbitrary; more repetitions slows down the
  ;; model, but too few gives poor layouts
  repeat 10 [
    do-layout
    display  ;; so we get smooth animation
  ]
end

to do-layout
  layout-spring nodes links 0.2 5 0.2
end
