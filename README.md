extensions [nw]

breed [nodes node]
nodes-own
[ID
  ;; this is used to mark turtles we have already visited
  explored?
 In_Links Out_links
  indeg
  outdeg
closeness
  betweenness
  eigenvector
  indeg0
  ki0 ki1 ki2 ki3 ki4 ki5 ki6 ki7 ki8 ki9 ki10 ki11 ki12 ki13 ki14 ki15 ki16 ki17 ki18 ki19 ki20 ki21 ki22 ki23 ki24 ki25 ki26
 ko0 ko1 ko2 ko3 ko4 ko5 ko6 ko7 ko8 ko9 ko10 ko11 ko12 ko13 ko14 ko15 ko16 ko17 ko18 ko19 ko20 ko21 ko22 ko23 ko24 ko25 ko26
 ODc0 ODc1 ODc2 ODc3 ODc4 ODc5 ODc6 ODc7 ODc8 ODc9 ODc10 ODc11 ODc12 ODc13 ODc14 ODc15 ODc16 ODc17 ODc18 ODc19 ODc20 ODc21 ODc22 ODc23 ODc24 ODc25 ODc26
 IDc0 IDc1 IDc2 IDc3 IDc4 IDc5 IDc6 IDc7 IDc8 IDc9 IDc10 IDc11 IDc12 IDc13 IDc14 IDc15 IDc16 IDc17 IDc18 IDc19 IDc20 IDc21 IDc22 IDc23 IDc24 IDc25 IDc26
 Cc0 Cc1 Cc2 Cc3 Cc4 Cc5 Cc6 Cc7 Cc8 Cc9 Cc10 Cc11 Cc12 Cc13 Cc14 Cc15 Cc16 Cc17 Cc18 Cc19 Cc20 Cc21 Cc22 Cc23 Cc24 Cc25 Cc26
 Bc0 Bc1 Bc2 Bc3 Bc4 Bc5 Bc6 Bc7 Bc8 Bc9 Bc10 Bc11 Bc12 Bc13 Bc14 Bc15 Bc16 Bc17 Bc18 Bc19 Bc20 Bc21 Bc22 Bc23 Bc24 Bc25 Bc26
 Ec0 Ec1 Ec2 Ec3 Ec4 Ec5 Ec6 Ec7 Ec8 Ec9 Ec10 Ec11 Ec12 Ec13 Ec14 Ec15 Ec16 Ec17 Ec18 Ec19 Ec20 Ec21 Ec22 Ec23 Ec24 Ec25 Ec26
  short
 short_i short_TR short_R short_F short_T short_n short_S short_Cp short_pHg short_Xg short_Cc short_foc short_pHw short_Tw short_pw short_Ew short_Iw short_Aw short_DOC short_pHm short_Tm short_pm short_Em short_Im short_Am short_t short_Xm
 short_0 short_1 short_2 short_3 short_4 short_5 short_6 short_7 short_8 short_9 short_10 short_11 short_12 short_13 short_14 short_15 short_16 short_17 short_18 short_19 short_20 short_21 short_22 short_23 short_24 short_25 short_26
 short_0_0 short_0_1 short_0_2 short_0_3 short_0_4 short_0_5 short_0_6 short_0_7 short_0_8 short_0_9 short_0_10 short_0_11 short_0_12 short_0_13 short_0_14 short_0_15 short_0_16 short_0_17 short_0_18 short_0_19 short_0_20 short_0_21 short_0_22 short_0_23 short_0_24 short_0_25 short_0_26
 short_1_0 short_1_1 short_1_2 short_1_3 short_1_4 short_1_5 short_1_6 short_1_7 short_1_8 short_1_9 short_1_10 short_1_11 short_1_12 short_1_13 short_1_14 short_1_15 short_1_16 short_1_17 short_1_18 short_1_19 short_1_20 short_1_21 short_1_22 short_1_23 short_1_24 short_1_25 short_1_26
 short_19_0 short_19_1 short_19_2 short_19_3 short_19_4 short_19_5 short_19_6 short_19_7 short_19_8 short_19_9 short_19_10 short_19_11 short_19_12 short_19_13 short_19_14 short_19_15 short_19_16 short_19_17 short_19_18 short_19_19 short_19_20 short_19_21 short_19_22 short_19_23 short_19_24 short_19_25 short_19_26
 short_20_0 short_20_1 short_20_2 short_20_3 short_20_4 short_20_5 short_20_6 short_20_7 short_20_8 short_20_9 short_20_10 short_20_11 short_20_12 short_20_13 short_20_14 short_20_15 short_20_16 short_20_17 short_20_18 short_20_19 short_20_20 short_20_21 short_20_22 short_20_23 short_20_24 short_20_25 short_20_26
 short_21_0 short_21_1 short_21_2 short_21_3 short_21_4 short_21_5 short_21_6 short_21_7 short_21_8 short_21_9 short_21_10 short_21_11 short_21_12 short_21_13 short_21_14 short_21_15 short_21_16 short_21_17 short_21_18 short_21_19 short_21_20 short_21_21 short_21_22 short_21_23 short_21_24 short_21_25 short_21_26
 short_22_0 short_22_1 short_22_2 short_22_3 short_22_4 short_22_5 short_22_6 short_22_7 short_22_8 short_22_9 short_22_10 short_22_11 short_22_12 short_22_13 short_22_14 short_22_15 short_22_16 short_22_17 short_22_18 short_22_19 short_22_20 short_22_21 short_22_22 short_22_23 short_22_24 short_22_25 short_22_26
 short_23_0 short_23_1 short_23_2 short_23_3 short_23_4 short_23_5 short_23_6 short_23_7 short_23_8 short_23_9 short_23_10 short_23_11 short_23_12 short_23_13 short_23_14 short_23_15 short_23_16 short_23_17 short_23_18 short_23_19 short_23_20 short_23_21 short_23_22 short_23_23 short_23_24 short_23_25 short_23_26
 short_24_0 short_24_1 short_24_2 short_24_3 short_24_4 short_24_5 short_24_6 short_24_7 short_24_8 short_24_9 short_24_10 short_24_11 short_24_12 short_24_13 short_24_14 short_24_15 short_24_16 short_24_17 short_24_18 short_24_19 short_24_20 short_24_21 short_24_22 short_24_23 short_24_24 short_24_25 short_24_26
 short_25_0 short_25_1 short_25_2 short_25_3 short_25_4 short_25_5 short_25_6 short_25_7 short_25_8 short_25_9 short_25_10 short_25_11 short_25_12 short_25_13 short_25_14 short_25_15 short_25_16 short_25_17 short_25_18 short_25_19 short_25_20 short_25_21 short_25_22 short_25_23 short_25_24 short_25_25 short_25_26
 short_26_0 short_26_1 short_26_2 short_26_3 short_26_4 short_26_5 short_26_6 short_26_7 short_26_8 short_26_9 short_26_10 short_26_11 short_26_12 short_26_13 short_26_14 short_26_15 short_26_16 short_26_17 short_26_18 short_26_19 short_26_20 short_26_21 short_26_22 short_26_23 short_26_24 short_26_25 short_26_26
 path
 path0 path1 path2 path3 path4 path5 path6 path7 path8 path9 path10 path11 path12 path13 path14 path15 path16 path17 path18 path19 path20 path21 path22 path23 path24 path25 path26
 j ;loop connector
 cluster0 cluster1 cluster2 cluster3 cluster4 cluster5 cluster6 cluster7 cluster8 cluster9 cluster10 cluster11 cluster12 cluster13 cluster14 cluster15 cluster16 cluster17 cluster18 cluster19 cluster20 cluster21 cluster22 cluster23 cluster24 cluster25 cluster26
]



globals
[
  component-size          ;; number of turtles explored so far in the current component
  giant-component-size    ;; number of turtles in the giant component
  giant-start-node        ;; node from where we started exploring the giant component
  pathlength              ;; sum of the path lengths between all nodes in the network
  Mean_cluster             ;; mean cluster of the network
  possiblepaths
  CharPL
  N
  L_in
  L_out


  ]


;;;;;;;;;;;;;;;;;;;;;;;;
;;; Setup Procedures ;;;
;;;;;;;;;;;;;;;;;;;;;;;;


to setup
  clear-all
  ask patches [
    set pcolor white
  ]

;Formation of nodes
;factor i
create-nodes 1[;who...0.....num-node-1
  set shape "circle"
  setxy random-pxcor random-pycor
  set color magenta
  ]

;factor TR
create-nodes 1[;who...0.....num-node-1
  set shape "circle"
  setxy random-pxcor random-pycor
  set color magenta
  ]

;factor R
create-nodes 1[;who...0.....num-node-1
  set shape "circle"
  setxy random-pxcor random-pycor
  set color green
  ]

;factor F
create-nodes 1[;who...0.....num-node-1
  set shape "circle"
  setxy random-pxcor random-pycor
  set color green
  ]

;factor T
create-nodes 1[;who...0.....num-node-1
  set shape "circle"
  setxy random-pxcor random-pycor
  set color lime
  ]

;factor n
create-nodes 1[;who...0.....num-node-1
  set shape "circle"
  setxy random-pxcor random-pycor
  set color lime
  ]

;factor S
create-nodes 1[;who...0.....num-node-1
  set shape "circle"
  setxy random-pxcor random-pycor
  set color lime
  ]

;factor Cp
create-nodes 1[;who...0.....num-node-1
  set shape "circle"
  setxy random-pxcor random-pycor
  set color lime
  ]

;factor pHg
create-nodes 1[;who...0.....num-node-1
  set shape "circle"
  setxy random-pxcor random-pycor
  set color orange
  ]

;factor Xg
create-nodes 1[;who...0.....num-node-1
  set shape "circle"
  setxy random-pxcor random-pycor
  set color orange
  ]

;factor Cc
create-nodes 1[;who...0.....num-node-1
  set shape "circle"
  setxy random-pxcor random-pycor
  set color orange
  ]

;factor foc
create-nodes 1[;who...0.....num-node-1
  set shape "circle"
  setxy random-pxcor random-pycor
  set color orange
  ]

;factor pHw
create-nodes 1[;who...0.....num-node-1
  set shape "circle"
  setxy random-pxcor random-pycor
  set color cyan
  ]

;factor Tw
create-nodes 1[;who...0.....num-node-1
  set shape "circle"
  setxy random-pxcor random-pycor
  set color cyan
  ]

;factor pw
create-nodes 1[;who...0.....num-node-1
  set shape "circle"
  setxy random-pxcor random-pycor
  set color cyan
  ]

;factor Ew
create-nodes 1[;who...0.....num-node-1
  set shape "circle"
  setxy random-pxcor random-pycor
  set color cyan
  ]

;factor Iw
create-nodes 1[;who...0.....num-node-1
  set shape "circle"
  setxy random-pxcor random-pycor
  set color cyan
  ]

;factor Aw
create-nodes 1[;who...0.....num-node-1
  set shape "circle"
  setxy random-pxcor random-pycor
  set color cyan
  ]

;factor DOC
create-nodes 1[;who...0.....num-node-1
  set shape "circle"
  setxy random-pxcor random-pycor
  set color cyan
  ]

;factor pHm
create-nodes 1[;who...0.....num-node-1
  set shape "circle"
  setxy random-pxcor random-pycor
  set color violet
  ]

;factor Tm
create-nodes 1[;who...0.....num-node-1
  set shape "circle"
  setxy random-pxcor random-pycor
  set color violet
  ]

;factor pm
create-nodes 1[;who...0.....num-node-1
  set shape "circle"
  setxy random-pxcor random-pycor
  set color violet
  ]

;factor Em
create-nodes 1[;who...0.....num-node-1
  set shape "circle"
  setxy random-pxcor random-pycor
  set color violet
  ]

;factor Im
create-nodes 1[;who...0.....num-node-1
  set shape "circle"
  setxy random-pxcor random-pycor
  set color violet
  ]

;factor Am
create-nodes 1[;who...0.....num-node-1
  set shape "circle"
  setxy random-pxcor random-pycor
  set color violet
  ]

;factor t
create-nodes 1[;who...0.....num-node-1
  set shape "circle"
  setxy random-pxcor random-pycor
  set color violet
  ]

;factor Xm
create-nodes 1[;who...0.....num-node-1
  set shape "circle"
  setxy random-pxcor random-pycor
  set color violet
  ]

;Formation of links between factors

  ;Links between i and other factors
  ask node 0 [ create-link-to node 2  ]
  ask node 0 [ create-link-to node 3  ]
  ask node 0 [ create-link-to node 7  ]
  ask node 0 [ create-link-to node 9  ]
  ask node 0 [ create-link-to node 19  ]
  ask node 0 [ create-link-to node 20  ]
  ask node 0 [ create-link-to node 21  ]
  ask node 0 [ create-link-to node 22  ]
  ask node 0 [ create-link-to node 23  ]
  ask node 0 [ create-link-to node 24  ]
  ask node 0 [ create-link-to node 26  ]

  ;Links between TR and other factors
  ask node 1 [ create-link-to node 0  ]
  ask node 1 [ create-link-to node 3  ]
  ask node 1 [ create-link-to node 9  ]
  ask node 1 [ create-link-to node 26  ]

  ;No out-going links from R to other factors



  ;Links between F and other factors
  ask node 3 [ create-link-to node 2  ]
  ask node 3 [ create-link-to node 6  ]
  ask node 3 [ create-link-to node 7  ]
  ask node 3 [ create-link-to node 9  ]
  ask node 3 [ create-link-to node 12  ]
  ask node 3 [ create-link-to node 13  ]
  ask node 3 [ create-link-to node 14  ]
  ask node 3 [ create-link-to node 15  ]
  ask node 3 [ create-link-to node 18  ]

  ;Links between T and other factors
  ask node 4 [ create-link-to node 5  ]
  ask node 4 [ create-link-to node 6  ]
  ask node 4 [ create-link-to node 7  ]
  ask node 4 [ create-link-to node 14  ]
  ask node 4 [ create-link-to node 15  ]
  ask node 4 [ create-link-to node 16  ]
  ask node 4 [ create-link-to node 17  ]
  ask node 4 [ create-link-to node 18  ]

  ;Links between n and other factors
  ask node 5 [ create-link-to node 3  ]
  ask node 5 [ create-link-to node 9  ]
  ask node 5 [ create-link-to node 14  ]
  ask node 5 [ create-link-to node 15  ]
  ask node 5 [ create-link-to node 16  ]
  ask node 5 [ create-link-to node 17  ]
  ask node 5 [ create-link-to node 18  ]

  ;Links between S and other factors
  ask node 6 [ create-link-to node 4  ]
  ask node 6 [ create-link-to node 7  ]
  ask node 6 [ create-link-to node 14 ]

  ;Links between Cp and other factors
  ask node 7 [ create-link-to node 3  ]
  ask node 7 [ create-link-to node 4  ]
  ask node 7 [ create-link-to node 5  ]
  ask node 7 [ create-link-to node 9  ]
  ask node 7 [ create-link-to node 10  ]
  ask node 7 [ create-link-to node 14  ]
  ask node 7 [ create-link-to node 15  ]

  ;Links between pHg and other factors
  ask node 8 [ create-link-to node 9  ]

  ;Links between Xg and other factors
  ask node 9 [ create-link-to node 4  ]
  ask node 9 [ create-link-to node 5  ]
  ask node 9 [ create-link-to node 11  ]
  ask node 9 [ create-link-to node 14  ]
  ask node 9 [ create-link-to node 15  ]
  ask node 9 [ create-link-to node 18  ]

  ;Links between Cc and other factors
  ask node 10 [ create-link-to node 8  ]
  ask node 10 [ create-link-to node 11  ]
  ask node 10 [ create-link-to node 14  ]
  ask node 10 [ create-link-to node 15  ]
  ask node 10 [ create-link-to node 16  ]
  ask node 10 [ create-link-to node 17  ]
  ask node 10 [ create-link-to node 18  ]

  ;Links between foc and other factors
  ask node 11 [ create-link-to node 2  ]
  ask node 11 [ create-link-to node 3  ]
  ask node 11 [ create-link-to node 6  ]
  ask node 11 [ create-link-to node 8  ]
  ask node 11 [ create-link-to node 9  ]
  ask node 11 [ create-link-to node 10  ]
  ask node 11 [ create-link-to node 12  ]
  ask node 11 [ create-link-to node 15  ]
  ask node 11 [ create-link-to node 18  ]

  ;Links between pHw and other factors
  ask node 12 [ create-link-to node 8  ]
  ask node 12 [ create-link-to node 9  ]
  ask node 12 [ create-link-to node 10  ]
  ask node 12 [ create-link-to node 15  ]
  ask node 12 [ create-link-to node 16  ]
  ask node 12 [ create-link-to node 17  ]
  ask node 12 [ create-link-to node 18  ]

  ;Links between Tw and other factors
  ask node 13 [ create-link-to node 9  ]
  ask node 13 [ create-link-to node 15  ]
  ask node 13 [ create-link-to node 16  ]

  ;Links between pw and other factors
  ask node 14 [ create-link-to node 4  ]
  ask node 14 [ create-link-to node 5  ]

  ;Links between Ew and other factors
  ask node 15 [ create-link-to node 9  ]

  ;Links between Iw and other factors
  ask node 16 [ create-link-to node 8  ]
  ask node 16 [ create-link-to node 10  ]
  ask node 16 [ create-link-to node 12  ]
  ask node 16 [ create-link-to node 14  ]
  ask node 16 [ create-link-to node 17  ]
  ask node 16 [ create-link-to node 18  ]

  ;Links between Aw and other factors
  ask node 17 [ create-link-to node 8  ]
  ask node 17 [ create-link-to node 9  ]
  ask node 17 [ create-link-to node 12  ]
  ask node 17 [ create-link-to node 16  ]
  ask node 17 [ create-link-to node 18  ]

  ;Links between DOC and other factors
  ask node 18 [ create-link-to node 8  ]
  ask node 18 [ create-link-to node 9  ]
  ask node 18 [ create-link-to node 12  ]
  ask node 18 [ create-link-to node 14  ]
  ask node 18 [ create-link-to node 15  ]
  ask node 18 [ create-link-to node 16  ]
  ask node 18 [ create-link-to node 17  ]

  ;Links between pHm and other factors
  ask node 19 [ create-link-to node 12  ]
  ask node 19 [ create-link-to node 21  ]
  ask node 19 [ create-link-to node 22  ]
  ask node 19 [ create-link-to node 26  ]

  ;Links between Tm and other factors
  ask node 20 [ create-link-to node 3  ]
  ask node 20 [ create-link-to node 13  ]
  ask node 20 [ create-link-to node 22  ]
  ask node 20 [ create-link-to node 23  ]
  ask node 20 [ create-link-to node 26  ]

  ;Links between pm and other factors
  ask node 21 [ create-link-to node 3  ]
  ask node 21 [ create-link-to node 4  ]
  ask node 21 [ create-link-to node 5  ]
  ask node 21 [ create-link-to node 9  ]
  ask node 21 [ create-link-to node 14  ]

  ;Links between Em and other factors
  ask node 22 [ create-link-to node 9  ]
  ask node 22 [ create-link-to node 15  ]
  ask node 22 [ create-link-to node 26  ]

  ;Links between Im and other factors
  ask node 23 [ create-link-to node 8  ]
  ask node 23 [ create-link-to node 12  ]
  ask node 23 [ create-link-to node 16  ]
  ask node 23 [ create-link-to node 21  ]
  ask node 23 [ create-link-to node 26  ]

  ;Links between Am and other factors
  ask node 24 [ create-link-to node 3  ]
  ask node 24 [ create-link-to node 17  ]
  ask node 24 [ create-link-to node 19  ]
  ask node 24 [ create-link-to node 23  ]
  ask node 24 [ create-link-to node 26  ]

  ;Links between t and other factors
  ask node 25 [ create-link-to node 19  ]
  ask node 25 [ create-link-to node 22  ]
  ask node 25 [ create-link-to node 23  ]
  ask node 25 [ create-link-to node 24  ]
  ask node 25 [ create-link-to node 26  ]

  ;Links between Xm and other factors
  ask node 26 [ create-link-to node 4  ]
  ask node 26 [ create-link-to node 5  ]
  ask node 26 [ create-link-to node 12  ]
  ask node 26 [ create-link-to node 14  ]
  ask node 26 [ create-link-to node 15  ]
  ask node 26 [ create-link-to node 19  ]
  ask node 26 [ create-link-to node 21  ]
  ask node 26 [ create-link-to node 22  ]
  ask node 26 [ create-link-to node 24  ]


find-all-components
color-giant-component

nw:set-context (nodes with [color = red] ) (links)

  print"This is a directed network"
  print "Number of factors in the NoF"
  set N count turtles
  show N
  print "Total number of incoming links"
  ask nodes [set In_Links count my-in-links]
  set L_in sum[In_Links] of nodes
  show L_in
  print "Total number of outgoing links"
  ask nodes [set Out_Links count my-out-links]
  set L_out sum[Out_Links] of nodes
  show L_out

;;;; Out-degree links of the factors ;;;;
  ;print "Out-degree value of factors"
  ask node 0 [set ko0 (count my-out-links)] ;show ko0]
  ask node 1 [set ko1 (count my-out-links)] ;show ko1]
  ask node 2 [set ko2 (count my-out-links)] ;show ko2]
  ask node 3 [set ko3 (count my-out-links)] ;show ko3]
  ask node 4 [set ko4 (count my-out-links)] ;show ko4]
  ask node 5 [set ko5 (count my-out-links)] ;show ko5]
  ask node 6 [set ko6 (count my-out-links)] ;show ko6]
  ask node 7 [set ko7 (count my-out-links)] ;show ko7]
  ask node 8 [set ko8 (count my-out-links)] ;show ko8]
  ask node 9 [set ko9 (count my-out-links)] ;show ko9]
  ask node 10 [set ko10 (count my-out-links)] ;show ko10]
  ask node 11 [set ko11 (count my-out-links)] ;show ko11]
  ask node 12 [set ko12 (count my-out-links)] ;show ko12]
  ask node 13 [set ko13 (count my-out-links)] ;show ko13]
  ask node 14 [set ko14 (count my-out-links)] ;show ko14]
  ask node 15 [set ko15 (count my-out-links)] ;show ko15]
  ask node 16 [set ko16 (count my-out-links)] ;show ko16]
  ask node 17 [set ko17 (count my-out-links)] ;show ko17]
  ask node 18 [set ko18 (count my-out-links)] ;show ko18]
  ask node 19 [set ko19 (count my-out-links)] ;show ko19]
  ask node 20 [set ko20 (count my-out-links)] ;show ko20]
  ask node 21 [set ko21 (count my-out-links)] ;show ko21]
  ask node 22 [set ko22 (count my-out-links)] ;show ko22]
  ask node 23 [set ko23 (count my-out-links)] ;show ko23]
  ask node 24 [set ko24 (count my-out-links)] ;show ko24]
  ask node 25 [set ko25 (count my-out-links)] ;show ko25]
  ask node 26 [set ko26 (count my-out-links)] ;show ko26]


;;;; In-degree links of the factors ;;;;
  ;print "In-degree value of factors"
  ask node 0 [set ki0 (count my-in-links)] ;show ki0]
  ask node 1 [set ki1 (count my-in-links)] ;show ki1]
  ask node 2 [set ki2 (count my-in-links)] ;show ki2]
  ask node 3 [set ki3 (count my-in-links)] ;show ki3]
  ask node 4 [set ki4 (count my-in-links)] ;show ki4]
  ask node 5 [set ki5 (count my-in-links)] ;show ki5]
  ask node 6 [set ki6 (count my-in-links)] ;show ki6]
  ask node 7 [set ki7 (count my-in-links)] ;show ki7]
  ask node 8 [set ki8 (count my-in-links)] ;show ki8]
  ask node 9 [set ki9 (count my-in-links)] ;show ki9]
  ask node 10 [set ki10 (count my-in-links)] ;show ki10]
  ask node 11 [set ki11 (count my-in-links)] ;show ki11]
  ask node 12 [set ki12 (count my-in-links)] ;show ki12]
  ask node 13 [set ki13 (count my-in-links)] ;show ki13]
  ask node 14 [set ki14 (count my-in-links)] ;show ki14]
  ask node 15 [set ki15 (count my-in-links)] ;show ki15]
  ask node 16 [set ki16 (count my-in-links)] ;show ki16]
  ask node 17 [set ki17 (count my-in-links)] ;show ki17]
  ask node 18 [set ki18 (count my-in-links)] ;show ki18]
  ask node 19 [set ki19 (count my-in-links)] ;show ki19]
  ask node 20 [set ki20 (count my-in-links)] ;show ki20]
  ask node 21 [set ki21 (count my-in-links)] ;show ki21]
  ask node 22 [set ki22 (count my-in-links)] ;show ki22]
  ask node 23 [set ki23 (count my-in-links)] ;show ki23]
  ask node 24 [set ki24 (count my-in-links)] ;show ki24]
  ask node 25 [set ki25 (count my-in-links)] ;show ki25]
  ask node 26 [set ki26 (count my-in-links)] ;show ki26]


;;;; Out-degree centrality ;;;;
  print "Out-degree centrality"
  ask node 0 [set ODc0 ( (ko0) / (N - 1) ) show ODc0]
  ask node 1 [set ODc1 ( (ko1) / (N - 1) ) show ODc1]
  ask node 2 [set ODc2 ( (ko2) / (N - 1) ) show ODc2]
  ask node 3 [set ODc3 ( (ko3) / (N - 1) ) show ODc3]
  ask node 4 [set ODc4 ( (ko4) / (N - 1) ) show ODc4]
  ask node 5 [set ODc5 ( (ko5) / (N - 1) ) show ODc5]
  ask node 6 [set ODc6 ( (ko6) / (N - 1) ) show ODc6]
  ask node 7 [set ODc7 ( (ko7) / (N - 1) ) show ODc7]
  ask node 8 [set ODc8 ( (ko8) / (N - 1) ) show ODc8]
  ask node 9 [set ODc9 ( (ko9) / (N - 1) ) show ODc9]
  ask node 10 [set ODc10 ( (ko10) / (N - 1) ) show ODc10]
  ask node 11 [set ODc11 ( (ko11) / (N - 1) ) show ODc11]
  ask node 12 [set ODc12 ( (ko12) / (N - 1) ) show ODc12]
  ask node 13 [set ODc13 ( (ko13) / (N - 1) ) show ODc13]
  ask node 14 [set ODc14 ( (ko14) / (N - 1) ) show ODc14]
  ask node 15 [set ODc15 ( (ko15) / (N - 1) ) show ODc15]
  ask node 16 [set ODc16 ( (ko16) / (N - 1) ) show ODc16]
  ask node 17 [set ODc17 ( (ko17) / (N - 1) ) show ODc17]
  ask node 18 [set ODc18 ( (ko18) / (N - 1) ) show ODc18]
  ask node 19 [set ODc19 ( (ko19) / (N - 1) ) show ODc19]
  ask node 20 [set ODc20 ( (ko20) / (N - 1) ) show ODc20]
  ask node 21 [set ODc21 ( (ko21) / (N - 1) ) show ODc21]
  ask node 22 [set ODc22 ( (ko22) / (N - 1) ) show ODc22]
  ask node 23 [set ODc23 ( (ko23) / (N - 1) ) show ODc23]
  ask node 24 [set ODc24 ( (ko24) / (N - 1) ) show ODc24]
  ask node 25 [set ODc25 ( (ko25) / (N - 1) ) show ODc25]
  ask node 26 [set ODc26 ( (ko26) / (N - 1) ) show ODc26]


;;;; In-degree centrality ;;;;
  print "In-degree centrality"
  ask node 0 [set IDc0 ( (ki0) / (N - 1) ) show IDc0]
ask node 1 [set IDc1 ( (ki1) / (N - 1) ) show IDc1]
ask node 2 [set IDc2 ( (ki2) / (N - 1) ) show IDc2]
ask node 3 [set IDc3 ( (ki3) / (N - 1) ) show IDc3]
ask node 4 [set IDc4 ( (ki4) / (N - 1) ) show IDc4]
ask node 5 [set IDc5 ( (ki5) / (N - 1) ) show IDc5]
ask node 6 [set IDc6 ( (ki6) / (N - 1) ) show IDc6]
ask node 7 [set IDc7 ( (ki7) / (N - 1) ) show IDc7]
ask node 8 [set IDc8 ( (ki8) / (N - 1) ) show IDc8]
ask node 9 [set IDc9 ( (ki9) / (N - 1) ) show IDc9]
ask node 10 [set IDc10 ( (ki10) / (N - 1) ) show IDc10]
ask node 11 [set IDc11 ( (ki11) / (N - 1) ) show IDc11]
ask node 12 [set IDc12 ( (ki12) / (N - 1) ) show IDc12]
ask node 13 [set IDc13 ( (ki13) / (N - 1) ) show IDc13]
ask node 14 [set IDc14 ( (ki14) / (N - 1) ) show IDc14]
ask node 15 [set IDc15 ( (ki15) / (N - 1) ) show IDc15]
ask node 16 [set IDc16 ( (ki16) / (N - 1) ) show IDc16]
ask node 17 [set IDc17 ( (ki17) / (N - 1) ) show IDc17]
ask node 18 [set IDc18 ( (ki18) / (N - 1) ) show IDc18]
ask node 19 [set IDc19 ( (ki19) / (N - 1) ) show IDc19]
ask node 20 [set IDc20 ( (ki20) / (N - 1) ) show IDc20]
ask node 21 [set IDc21 ( (ki21) / (N - 1) ) show IDc21]
ask node 22 [set IDc22 ( (ki22) / (N - 1) ) show IDc22]
ask node 23 [set IDc23 ( (ki23) / (N - 1) ) show IDc23]
ask node 24 [set IDc24 ( (ki24) / (N - 1) ) show IDc24]
ask node 25 [set IDc25 ( (ki25) / (N - 1) )show IDc25]
ask node 26 [set IDc26 ( (ki26) / (N - 1) ) show IDc26]


;;;; Closeness centrality ;;;;
 print "Closeness centrality"
  ask node 0 [set Cc0 nw:closeness-centrality show Cc0]
ask node 1 [set Cc1 nw:closeness-centrality show Cc1]
ask node 2 [set Cc2 nw:closeness-centrality show Cc2]
ask node 3 [set Cc3 nw:closeness-centrality show Cc3]
ask node 4 [set Cc4 nw:closeness-centrality show Cc4]
ask node 5 [set Cc5 nw:closeness-centrality show Cc5]
ask node 6 [set Cc6 nw:closeness-centrality show Cc6]
ask node 7 [set Cc7 nw:closeness-centrality show Cc7]
ask node 8 [set Cc8 nw:closeness-centrality show Cc8]
ask node 9 [set Cc9 nw:closeness-centrality show Cc9]
ask node 10 [set Cc10 nw:closeness-centrality show Cc10]
ask node 11 [set Cc11 nw:closeness-centrality show Cc11]
ask node 12 [set Cc12 nw:closeness-centrality show Cc12]
ask node 13 [set Cc13 nw:closeness-centrality show Cc13]
ask node 14 [set Cc14 nw:closeness-centrality show Cc14]
ask node 15 [set Cc15 nw:closeness-centrality show Cc15]
ask node 16 [set Cc16 nw:closeness-centrality show Cc16]
ask node 17 [set Cc17 nw:closeness-centrality show Cc17]
ask node 18 [set Cc18 nw:closeness-centrality show Cc18]
ask node 19 [set Cc19 nw:closeness-centrality show Cc19]
ask node 20 [set Cc20 nw:closeness-centrality show Cc20]
ask node 21 [set Cc21 nw:closeness-centrality show Cc21]
ask node 22 [set Cc22 nw:closeness-centrality show Cc22]
ask node 23 [set Cc23 nw:closeness-centrality show Cc23]
ask node 24 [set Cc24 nw:closeness-centrality show Cc24]
ask node 25 [set Cc25 nw:closeness-centrality show Cc25]
ask node 26 [set Cc26 nw:closeness-centrality show Cc26]


;;;; Betweenness centrality ;;;;
  print "Betweenness centrality"
ask node 0 [set Bc0 nw:betweenness-centrality show Bc0]
ask node 1 [set Bc1 nw:betweenness-centrality show Bc1]
ask node 2 [set Bc2 nw:betweenness-centrality show Bc2]
ask node 3 [set Bc3 nw:betweenness-centrality show Bc3]
ask node 4 [set Bc4 nw:betweenness-centrality show Bc4]
ask node 5 [set Bc5 nw:betweenness-centrality show Bc5]
ask node 6 [set Bc6 nw:betweenness-centrality show Bc6]
ask node 7 [set Bc7 nw:betweenness-centrality show Bc7]
ask node 8 [set Bc8 nw:betweenness-centrality show Bc8]
ask node 9 [set Bc9 nw:betweenness-centrality show Bc9]
ask node 10 [set Bc10 nw:betweenness-centrality show Bc10]
ask node 11 [set Bc11 nw:betweenness-centrality show Bc11]
ask node 12 [set Bc12 nw:betweenness-centrality show Bc12]
ask node 13 [set Bc13 nw:betweenness-centrality show Bc13]
ask node 14 [set Bc14 nw:betweenness-centrality show Bc14]
ask node 15 [set Bc15 nw:betweenness-centrality show Bc15]
ask node 16 [set Bc16 nw:betweenness-centrality show Bc16]
ask node 17 [set Bc17 nw:betweenness-centrality show Bc17]
ask node 18 [set Bc18 nw:betweenness-centrality show Bc18]
ask node 19 [set Bc19 nw:betweenness-centrality show Bc19]
ask node 20 [set Bc20 nw:betweenness-centrality show Bc20]
ask node 21 [set Bc21 nw:betweenness-centrality show Bc21]
ask node 22 [set Bc22 nw:betweenness-centrality show Bc22]
ask node 23 [set Bc23 nw:betweenness-centrality show Bc23]
ask node 24 [set Bc24 nw:betweenness-centrality show Bc24]
ask node 25 [set Bc25 nw:betweenness-centrality show Bc25]
ask node 26 [set Bc26 nw:betweenness-centrality show Bc26]

;;;; Eigenvector centrality ;;;;
  print "Eigenvector centrality"
  ask node 0 [set Ec0 nw:eigenvector-centrality show Ec0]
  ask node 1 [set Ec1 nw:eigenvector-centrality show Ec1]
  ask node 2 [set Ec2 nw:eigenvector-centrality show Ec2]
  ask node 3 [set Ec3 nw:eigenvector-centrality show Ec3]
  ask node 4 [set Ec4 nw:eigenvector-centrality show Ec4]
  ask node 5 [set Ec5 nw:eigenvector-centrality show Ec5]
  ask node 6 [set Ec6 nw:eigenvector-centrality show Ec6]
  ask node 7 [set Ec7 nw:eigenvector-centrality show Ec7]
  ask node 8 [set Ec8 nw:eigenvector-centrality show Ec8]
  ask node 9 [set Ec9 nw:eigenvector-centrality show Ec9]
  ask node 10 [set Ec10 nw:eigenvector-centrality show Ec10]
  ask node 11 [set Ec11 nw:eigenvector-centrality show Ec11]
  ask node 12 [set Ec12 nw:eigenvector-centrality show Ec12]
  ask node 13 [set Ec13 nw:eigenvector-centrality show Ec13]
  ask node 14 [set Ec14 nw:eigenvector-centrality show Ec14]
  ask node 15 [set Ec15 nw:eigenvector-centrality show Ec15]
  ask node 16 [set Ec16 nw:eigenvector-centrality show Ec16]
  ask node 17 [set Ec17 nw:eigenvector-centrality show Ec17]
  ask node 18 [set Ec18 nw:eigenvector-centrality show Ec18]
  ask node 19 [set Ec19 nw:eigenvector-centrality show Ec19]
  ask node 20 [set Ec20 nw:eigenvector-centrality show Ec20]
  ask node 21 [set Ec21 nw:eigenvector-centrality show Ec21]
  ask node 22 [set Ec22 nw:eigenvector-centrality show Ec22]
  ask node 23 [set Ec23 nw:eigenvector-centrality show Ec23]
  ask node 24 [set Ec24 nw:eigenvector-centrality show Ec24]
  ask node 25 [set Ec25 nw:eigenvector-centrality show Ec25]
  ask node 26 [set Ec26 nw:eigenvector-centrality show Ec26]


;;;; Characteristic pathlength ;;;;

;; Finding paths between node 0 and other factors

  ask node 0 [set short_0_0 nw:distance-to node 0]
  ask node 0 [set short_0_1 nw:distance-to node 1]
  ask node 0 [set short_0_2 nw:distance-to node 2]
  ask node 0 [set short_0_3 nw:distance-to node 3]
  ask node 0 [set short_0_4 nw:distance-to node 4]
  ask node 0 [set short_0_5 nw:distance-to node 5]
  ask node 0 [set short_0_6 nw:distance-to node 6]
  ask node 0 [set short_0_7 nw:distance-to node 7]
  ask node 0 [set short_0_8 nw:distance-to node 8]
  ask node 0 [set short_0_9 nw:distance-to node 9]
  ask node 0 [set short_0_10 nw:distance-to node 10]
  ask node 0 [set short_0_11 nw:distance-to node 11]
  ask node 0 [set short_0_12 nw:distance-to node 12]
  ask node 0 [set short_0_13 nw:distance-to node 13]
  ask node 0 [set short_0_14 nw:distance-to node 14]
  ask node 0 [set short_0_15 nw:distance-to node 15]
  ask node 0 [set short_0_16 nw:distance-to node 16]
  ask node 0 [set short_0_17 nw:distance-to node 17]
  ask node 0 [set short_0_18 nw:distance-to node 18]
  ask node 0 [set short_0_19 nw:distance-to node 19]
  ask node 0 [set short_0_20 nw:distance-to node 20]
  ask node 0 [set short_0_21 nw:distance-to node 21]
  ask node 0 [set short_0_22 nw:distance-to node 22]
  ask node 0 [set short_0_23 nw:distance-to node 23]
  ask node 0 [set short_0_24 nw:distance-to node 24]
  ask node 0 [set short_0_25 nw:distance-to node 25]
  ask node 0 [set short_0_26 nw:distance-to node 26]

 ;ask node 0 [show short_0_0 show short_0_1 show short_0_2 show short_0_3 show short_0_4 show short_0_5 show short_0_6 show short_0_7 show short_0_8 show short_0_9 show short_0_10 show short_0_11 show short_0_12 show short_0_13 show short_0_14 show short_0_15 show short_0_16 show short_0_17 show short_0_18 show short_0_19 show short_0_20 show short_0_21 show short_0_22 show short_0_23 show short_0_24 show short_0_25 show short_0_26]

; If there is a path then path , the value is returned as false then the path is 0.
; In the following case, there is no path for a factor to itself.

  ask node 0 [ set path0 0 ]
  ask node 0 [ifelse (short_0_0 = false) [set short_0_0 0] [set short_0_0 short_0_0] ]
; checking if there is a path between node 0 and 1 and so on
  ask node 0 [ifelse (short_0_1 = false) [set short_0_1 0] [set short_0_1 short_0_1 set path0 path0 + 1] ]
  ask node 0 [ifelse (short_0_2 = false) [set short_0_2 0] [set short_0_2 short_0_2 set path0 path0 + 1] ]
  ask node 0 [ifelse (short_0_3 = false) [set short_0_3 0] [set short_0_3 short_0_3 set path0 path0 + 1] ]
  ask node 0 [ifelse (short_0_4 = false) [set short_0_4 0] [set short_0_4 short_0_4 set path0 path0 + 1] ]
  ask node 0 [ifelse (short_0_5 = false) [set short_0_5 0] [set short_0_5 short_0_5 set path0 path0 + 1] ]
  ask node 0 [ifelse (short_0_6 = false) [set short_0_6 0] [set short_0_6 short_0_6 set path0 path0 + 1] ]
  ask node 0 [ifelse (short_0_7 = false) [set short_0_7 0] [set short_0_7 short_0_7 set path0 path0 + 1] ]
  ask node 0 [ifelse (short_0_8 = false) [set short_0_8 0] [set short_0_8 short_0_8 set path0 path0 + 1] ]
  ask node 0 [ifelse (short_0_9 = false) [set short_0_9 0] [set short_0_9 short_0_9 set path0 path0 + 1] ]
  ask node 0 [ifelse (short_0_10 = false) [set short_0_10 0] [set short_0_10 short_0_10 set path0 path0 + 1] ]
  ask node 0 [ifelse (short_0_11 = false) [set short_0_11 0] [set short_0_11 short_0_11 set path0 path0 + 1] ]
  ask node 0 [ifelse (short_0_12 = false) [set short_0_12 0] [set short_0_12 short_0_12 set path0 path0 + 1] ]
  ask node 0 [ifelse (short_0_13 = false) [set short_0_13 0] [set short_0_13 short_0_13 set path0 path0 + 1] ]
  ask node 0 [ifelse (short_0_14 = false) [set short_0_14 0] [set short_0_14 short_0_14 set path0 path0 + 1] ]
  ask node 0 [ifelse (short_0_15 = false) [set short_0_15 0] [set short_0_15 short_0_15 set path0 path0 + 1] ]
  ask node 0 [ifelse (short_0_16 = false) [set short_0_16 0] [set short_0_16 short_0_16 set path0 path0 + 1] ]
  ask node 0 [ifelse (short_0_17 = false) [set short_0_17 0] [set short_0_17 short_0_17 set path0 path0 + 1] ]
  ask node 0 [ifelse (short_0_18 = false) [set short_0_18 0] [set short_0_18 short_0_18 set path0 path0 + 1] ]
  ask node 0 [ifelse (short_0_19 = false) [set short_0_19 0] [set short_0_19 short_0_19 set path0 path0 + 1] ]
  ask node 0 [ifelse (short_0_20 = false) [set short_0_20 0] [set short_0_20 short_0_20 set path0 path0 + 1] ]
  ask node 0 [ifelse (short_0_21 = false) [set short_0_21 0] [set short_0_21 short_0_21 set path0 path0 + 1] ]
  ask node 0 [ifelse (short_0_22 = false) [set short_0_22 0] [set short_0_22 short_0_22 set path0 path0 + 1] ]
  ask node 0 [ifelse (short_0_23 = false) [set short_0_23 0] [set short_0_23 short_0_23 set path0 path0 + 1] ]
  ask node 0 [ifelse (short_0_24 = false) [set short_0_24 0] [set short_0_24 short_0_24 set path0 path0 + 1] ]
  ask node 0 [ifelse (short_0_25 = false) [set short_0_25 0] [set short_0_25 short_0_25 set path0 path0 + 1] ]
  ask node 0 [ifelse (short_0_26 = false) [set short_0_26 0] [set short_0_26 short_0_26 set path0 path0 + 1] ]

 ; ask node 0 [show path0] ;path verified ;24 other nodes in the NoF show possible paths with node 0 hence the total paths from node 0 is 24

;; Finding paths between node 1 and other factors

  ask node 1 [set short_1_0 nw:distance-to node 0]
  ask node 1 [set short_1_1 nw:distance-to node 1]
  ask node 1 [set short_1_2 nw:distance-to node 2]
  ask node 1 [set short_1_3 nw:distance-to node 3]
  ask node 1 [set short_1_4 nw:distance-to node 4]
  ask node 1 [set short_1_5 nw:distance-to node 5]
  ask node 1 [set short_1_6 nw:distance-to node 6]
  ask node 1 [set short_1_7 nw:distance-to node 7]
  ask node 1 [set short_1_8 nw:distance-to node 8]
  ask node 1 [set short_1_9 nw:distance-to node 9]
  ask node 1 [set short_1_10 nw:distance-to node 10]
  ask node 1 [set short_1_11 nw:distance-to node 11]
  ask node 1 [set short_1_12 nw:distance-to node 12]
  ask node 1 [set short_1_13 nw:distance-to node 13]
  ask node 1 [set short_1_14 nw:distance-to node 14]
  ask node 1 [set short_1_15 nw:distance-to node 15]
  ask node 1 [set short_1_16 nw:distance-to node 16]
  ask node 1 [set short_1_17 nw:distance-to node 17]
  ask node 1 [set short_1_18 nw:distance-to node 18]
  ask node 1 [set short_1_19 nw:distance-to node 19]
  ask node 1 [set short_1_20 nw:distance-to node 20]
  ask node 1 [set short_1_21 nw:distance-to node 21]
  ask node 1 [set short_1_22 nw:distance-to node 22]
  ask node 1 [set short_1_23 nw:distance-to node 23]
  ask node 1 [set short_1_24 nw:distance-to node 24]
  ask node 1 [set short_1_25 nw:distance-to node 25]
  ask node 1 [set short_1_26 nw:distance-to node 26]

 ;ask node 1 [show short_1_0 show short_1_1 show short_1_2 show short_1_3 show short_1_4 show short_1_5 show short_1_6 show short_1_7 show short_1_8 show short_1_9 show short_1_10 show short_1_11 show short_1_12 show short_1_13 show short_1_14 show short_1_15 show short_1_16 show short_1_17 show short_1_18 show short_1_19 show short_1_20 show short_1_21 show short_1_22 show short_1_23 show short_1_24 show short_1_25 show short_1_26]

; If there is a path then path value is incremented. If the value is returned as false/zero then the path is 0.
; There is no path for a factor to itself.

  ask node 1 [ set path1 0 ]
  ask node 1 [ifelse (short_1_0 = false) [set short_1_0 0] [set short_1_0 short_1_0 set path1 path1 + 1] ]
; checking if there is a path between node 0 and 1 and so on
  ask node 1 [ifelse (short_1_1 = false) [set short_1_1 0] [set short_1_1 short_1_1] ]
  ask node 1 [ifelse (short_1_2 = false) [set short_1_2 0] [set short_1_2 short_1_2 set path1 path1 + 1] ]
  ask node 1 [ifelse (short_1_3 = false) [set short_1_3 0] [set short_1_3 short_1_3 set path1 path1 + 1] ]
  ask node 1 [ifelse (short_1_4 = false) [set short_1_4 0] [set short_1_4 short_1_4 set path1 path1 + 1] ]
  ask node 1 [ifelse (short_1_5 = false) [set short_1_5 0] [set short_1_5 short_1_5 set path1 path1 + 1] ]
  ask node 1 [ifelse (short_1_6 = false) [set short_1_6 0] [set short_1_6 short_1_6 set path1 path1 + 1] ]
  ask node 1 [ifelse (short_1_7 = false) [set short_1_7 0] [set short_1_7 short_1_7 set path1 path1 + 1] ]
  ask node 1 [ifelse (short_1_8 = false) [set short_1_8 0] [set short_1_8 short_1_8 set path1 path1 + 1] ]
  ask node 1 [ifelse (short_1_9 = false) [set short_1_9 0] [set short_1_9 short_1_9 set path1 path1 + 1] ]
  ask node 1 [ifelse (short_1_10 = false) [set short_1_10 0] [set short_1_10 short_1_10 set path1 path1 + 1] ]
  ask node 1 [ifelse (short_1_11 = false) [set short_1_11 0] [set short_1_11 short_1_11 set path1 path1 + 1] ]
  ask node 1 [ifelse (short_1_12 = false) [set short_1_12 0] [set short_1_12 short_1_12 set path1 path1 + 1] ]
  ask node 1 [ifelse (short_1_13 = false) [set short_1_13 0] [set short_1_13 short_1_13 set path1 path1 + 1] ]
  ask node 1 [ifelse (short_1_14 = false) [set short_1_14 0] [set short_1_14 short_1_14 set path1 path1 + 1] ]
  ask node 1 [ifelse (short_1_15 = false) [set short_1_15 0] [set short_1_15 short_1_15 set path1 path1 + 1] ]
  ask node 1 [ifelse (short_1_16 = false) [set short_1_16 0] [set short_1_16 short_1_16 set path1 path1 + 1] ]
  ask node 1 [ifelse (short_1_17 = false) [set short_1_17 0] [set short_1_17 short_1_17 set path1 path1 + 1] ]
  ask node 1 [ifelse (short_1_18 = false) [set short_1_18 0] [set short_1_18 short_1_18 set path1 path1 + 1] ]
  ask node 1 [ifelse (short_1_19 = false) [set short_1_19 0] [set short_1_19 short_1_19 set path1 path1 + 1] ]
  ask node 1 [ifelse (short_1_20 = false) [set short_1_20 0] [set short_1_20 short_1_20 set path1 path1 + 1] ]
  ask node 1 [ifelse (short_1_21 = false) [set short_1_21 0] [set short_1_21 short_1_21 set path1 path1 + 1] ]
  ask node 1 [ifelse (short_1_22 = false) [set short_1_22 0] [set short_1_22 short_1_22 set path1 path1 + 1] ]
  ask node 1 [ifelse (short_1_23 = false) [set short_1_23 0] [set short_1_23 short_1_23 set path1 path1 + 1] ]
  ask node 1 [ifelse (short_1_24 = false) [set short_1_24 0] [set short_1_24 short_1_24 set path1 path1 + 1] ]
  ask node 1 [ifelse (short_1_25 = false) [set short_1_25 0] [set short_1_25 short_1_25 set path1 path1 + 1] ]
  ask node 1 [ifelse (short_1_26 = false) [set short_1_26 0] [set short_1_26 short_1_26 set path1 path1 + 1] ]

 ;ask node 1 [show path1] ;path verified ;25 other nodes in the NoF show possible paths with node 1 hence the total paths from node 1 is 25.


;; Finding paths between node 2 and other factors
  ask nodes [set short_2 nw:distance-to node 2]
  ;ask nodes [show short_2]

  ask node 2 [ set j 0 set path2 0
    loop [ ifelse (j = 27) [ stop ] [if (nw:distance-to node j != 0) [set path2 path2 + 1] ] set j j + 1] ]
; ask node 2 [ show path2 ] ;path verified ;26 other nodes in the NoF show possible paths with this node.


;; Finding paths between node 3 and other factors
  ask nodes [set short_3 nw:distance-to node 3]
 ; ask nodes [show short_3]

  ask node 3 [ set j 0 set path3 0
    loop [ ifelse (j = 27) [ stop ] [if (nw:distance-to node j != 0) [set path3 path3 + 1] ] set j j + 1] ]
 ;ask node 3 [ show path3 ] ;path verified ;26 other nodes in the NoF show possible paths with this node.


;; Finding paths between node 4 and other factors
  ask nodes [set short_4 nw:distance-to node 4]
  ;ask nodes [show short_4]

  ask node 4 [ set j 0 set path4 0
    loop [ ifelse (j = 27) [ stop ] [if (nw:distance-to node j != 0) [set path4 path4 + 1] ] set j j + 1] ]
 ;ask node 4 [ show path4 ] ;path verified ;26 other nodes in the NoF show possible paths with this node.


;; Finding paths between node 5 and other factors
  ask nodes [set short_5 nw:distance-to node 5]
 ; ask nodes [show short_5]

  ask node 5 [ set j 0 set path5 0
    loop [ ifelse (j = 27) [ stop ] [if (nw:distance-to node j != 0) [set path5 path5 + 1] ] set j j + 1] ]
; ask node 5 [ show path5 ] ;path verified ;26 other nodes in the NoF show possible paths with this node.


;; Finding paths between node 6 and other factors
  ask nodes [set short_6 nw:distance-to node 6]
 ;ask nodes [show short_6]

  ask node 6 [ set j 0 set path6 0
    loop [ ifelse (j = 27) [ stop ] [if (nw:distance-to node j != 0) [set path6 path6 + 1] ] set j j + 1] ]
 ;ask node 6 [ show path6 ] ;path verified ;26 other nodes in the NoF show possible paths with this node.


;; Finding paths between node 7 and other factors
  ask nodes [set short_7 nw:distance-to node 7]
 ;ask nodes [show short_7]

  ask node 7 [ set j 0 set path7 0
    loop [ ifelse (j = 27) [ stop ] [if (nw:distance-to node j != 0) [set path7 path7 + 1] ] set j j + 1] ]
 ;ask node 7 [ show path7 ] ;path verified ;26 other nodes in the NoF show possible paths with this node.


;; Finding paths between node 8 and other factors
  ask nodes [set short_8 nw:distance-to node 8]
  ;ask nodes [show short_8]

  ask node 8 [ set j 0 set path8 0
    loop [ ifelse (j = 27) [ stop ] [if (nw:distance-to node j != 0) [set path8 path8 + 1] ] set j j + 1] ]
 ;ask node 8 [ show path8 ] ;path verified ;26 other nodes in the NoF show possible paths with this node.


;; Finding paths between node 9 and other factors
  ask nodes [set short_9 nw:distance-to node 9]
  ;ask nodes [show short_9]

  ask node 9 [ set j 0 set path9 0
    loop [ ifelse (j = 27) [ stop ] [if (nw:distance-to node j != 0) [set path9 path9 + 1] ] set j j + 1] ]
 ;ask node 9 [ show path9 ] ;path verified ;26 other nodes in the NoF show possible paths with this node.


;; Finding paths between node 10 and other factors
  ask nodes [set short_10 nw:distance-to node 10]
 ; ask nodes [show short_10]

  ask node 10 [ set j 0 set path10 0
    loop [ ifelse (j = 27) [ stop ] [if (nw:distance-to node j != 0) [set path10 path10 + 1] ] set j j + 1] ]
 ;ask node 10 [ show path10 ] ;path verified ;26 other nodes in the NoF show possible paths with this node.


;; Finding paths between node 11 and other factors
  ask nodes [set short_11 nw:distance-to node 11]
 ; ask nodes [show short_11]

  ask node 11 [ set j 0 set path11 0
    loop [ ifelse (j = 27) [ stop ] [if (nw:distance-to node j != 0) [set path11 path11 + 1] ] set j j + 1] ]
; ask node 11 [ show path11 ] ;path verified ;26 other nodes in the NoF show possible paths with this node.


;; Finding paths between node 12 and other factors
  ask nodes [set short_12 nw:distance-to node 12]
 ;ask nodes [show short_12]

  ask node 12 [ set j 0 set path12 0
    loop [ ifelse (j = 27) [ stop ] [if (nw:distance-to node j != 0) [set path12 path12 + 1] ] set j j + 1] ]
 ;ask node 12 [ show path12 ] ;path verified ;26 other nodes in the NoF show possible paths with this node.


;; Finding paths between node 13 and other factors
  ask nodes [set short_13 nw:distance-to node 13]
 ; ask nodes [show short_13]

  ask node 13 [ set j 0 set path13 0
    loop [ ifelse (j = 27) [ stop ] [if (nw:distance-to node j != 0) [set path13 path13 + 1] ] set j j + 1] ]
 ;ask node 13 [ show path13 ] ;path verified ;26 other nodes in the NoF show possible paths with this node.


;; Finding paths between node 14 and other factors
  ask nodes [set short_14 nw:distance-to node 14]
 ; ask nodes [show short_14]

  ask node 14 [ set j 0 set path14 0
    loop [ ifelse (j = 27) [ stop ] [if (nw:distance-to node j != 0) [set path14 path14 + 1] ] set j j + 1] ]
; ask node 14 [ show path14 ] ;path verified ;26 other nodes in the NoF show possible paths with this node.


;; Finding paths between node 15 and other factors
  ask nodes [set short_15 nw:distance-to node 15]
 ;ask nodes [show short_15]

  ask node 15 [ set j 0 set path15 0
    loop [ ifelse (j = 27) [ stop ] [if (nw:distance-to node j != 0) [set path15 path15 + 1] ] set j j + 1] ]
 ;ask node 15 [ show path15 ] ;path verified ;26 other nodes in the NoF show possible paths with this node.


;; Finding paths between node 16 and other factors
  ask nodes [set short_16 nw:distance-to node 16]
 ; ask nodes [show short_16]

  ask node 16 [ set j 0 set path16 0
    loop [ ifelse (j = 27) [ stop ] [if (nw:distance-to node j != 0) [set path16 path16 + 1] ] set j j + 1] ]
 ;ask node 16 [ show path16 ] ;path verified ;26 other nodes in the NoF show possible paths with this node.


;; Finding paths between node 17 and other factors
  ask nodes [set short_17 nw:distance-to node 17]
 ;ask nodes [show short_17]

  ask node 17 [ set j 0 set path17 0
    loop [ ifelse (j = 27) [ stop ] [if (nw:distance-to node j != 0) [set path17 path17 + 1] ] set j j + 1] ]
 ;ask node 17 [ show path17 ] ;path verified ;26 other nodes in the NoF show possible paths with this node.


;; Finding paths between node 18 and other factors
  ask nodes [set short_18 nw:distance-to node 18]
 ;ask nodes [show short_18]

  ask node 18 [ set j 0 set path18 0
    loop [ ifelse (j = 27) [ stop ] [if (nw:distance-to node j != 0) [set path18 path18 + 1] ] set j j + 1] ]
 ;ask node 18 [ show path18 ] ;path verified ;26 other nodes in the NoF show possible paths with this node.


;; Finding paths between node 19 and other factors

  ask node 19 [set short_19_0 nw:distance-to node 0]
  ask node 19 [set short_19_1 nw:distance-to node 1]
  ask node 19 [set short_19_2 nw:distance-to node 2]
  ask node 19 [set short_19_3 nw:distance-to node 3]
  ask node 19 [set short_19_4 nw:distance-to node 4]
  ask node 19 [set short_19_5 nw:distance-to node 5]
  ask node 19 [set short_19_6 nw:distance-to node 6]
  ask node 19 [set short_19_7 nw:distance-to node 7]
  ask node 19 [set short_19_8 nw:distance-to node 8]
  ask node 19 [set short_19_9 nw:distance-to node 9]
  ask node 19 [set short_19_10 nw:distance-to node 10]
  ask node 19 [set short_19_11 nw:distance-to node 11]
  ask node 19 [set short_19_12 nw:distance-to node 12]
  ask node 19 [set short_19_13 nw:distance-to node 13]
  ask node 19 [set short_19_14 nw:distance-to node 14]
  ask node 19 [set short_19_15 nw:distance-to node 15]
  ask node 19 [set short_19_16 nw:distance-to node 16]
  ask node 19 [set short_19_17 nw:distance-to node 17]
  ask node 19 [set short_19_18 nw:distance-to node 18]
  ask node 19 [set short_19_19 nw:distance-to node 19]
  ask node 19 [set short_19_20 nw:distance-to node 20]
  ask node 19 [set short_19_21 nw:distance-to node 21]
  ask node 19 [set short_19_22 nw:distance-to node 22]
  ask node 19 [set short_19_23 nw:distance-to node 23]
  ask node 19 [set short_19_24 nw:distance-to node 24]
  ask node 19 [set short_19_25 nw:distance-to node 25]
  ask node 19 [set short_19_26 nw:distance-to node 26]

; ask node 19 [show short_19_0 show short_19_1 show short_19_2 show short_19_3 show short_19_4 show short_19_5 show short_19_6 show short_19_7 show short_19_8 show short_19_9 show short_19_10 show short_19_11 show short_19_12 show short_19_13 show short_19_14 show short_19_15 show short_19_16 show short_19_17 show short_19_18 show short_19_19 show short_19_20 show short_19_21 show short_19_22 show short_19_23 show short_19_24 show short_19_25 show short_19_26]

  ask node 19 [ set path19 0 ]
  ask node 19 [ifelse (short_19_0 = false) [set short_19_0 0] [set short_19_0 short_19_0 set path19 path19 + 1] ]
  ask node 19 [ifelse (short_19_1 = false) [set short_19_1 0] [set short_19_1 short_19_1 set path19 path19 + 1] ]
  ask node 19 [ifelse (short_19_2 = false) [set short_19_2 0] [set short_19_2 short_19_2 set path19 path19 + 1] ]
  ask node 19 [ifelse (short_19_3 = false) [set short_19_3 0] [set short_19_3 short_19_3 set path19 path19 + 1] ]
  ask node 19 [ifelse (short_19_4 = false) [set short_19_4 0] [set short_19_4 short_19_4 set path19 path19 + 1] ]
  ask node 19 [ifelse (short_19_5 = false) [set short_19_5 0] [set short_19_5 short_19_5 set path19 path19 + 1] ]
  ask node 19 [ifelse (short_19_6 = false) [set short_19_6 0] [set short_19_6 short_19_6 set path19 path19 + 1] ]
  ask node 19 [ifelse (short_19_7 = false) [set short_19_7 0] [set short_19_7 short_19_7 set path19 path19 + 1] ]
  ask node 19 [ifelse (short_19_8 = false) [set short_19_8 0] [set short_19_8 short_19_8 set path19 path19 + 1] ]
  ask node 19 [ifelse (short_19_9 = false) [set short_19_9 0] [set short_19_9 short_19_9 set path19 path19 + 1] ]
  ask node 19 [ifelse (short_19_10 = false) [set short_19_10 0] [set short_19_10 short_19_10 set path19 path19 + 1] ]
  ask node 19 [ifelse (short_19_11 = false) [set short_19_11 0] [set short_19_11 short_19_11 set path19 path19 + 1] ]
  ask node 19 [ifelse (short_19_12 = false) [set short_19_12 0] [set short_19_12 short_19_12 set path19 path19 + 1] ]
  ask node 19 [ifelse (short_19_13 = false) [set short_19_13 0] [set short_19_13 short_19_13 set path19 path19 + 1] ]
  ask node 19 [ifelse (short_19_14 = false) [set short_19_14 0] [set short_19_14 short_19_14 set path19 path19 + 1] ]
  ask node 19 [ifelse (short_19_15 = false) [set short_19_15 0] [set short_19_15 short_19_15 set path19 path19 + 1] ]
  ask node 19 [ifelse (short_19_16 = false) [set short_19_16 0] [set short_19_16 short_19_16 set path19 path19 + 1] ]
  ask node 19 [ifelse (short_19_17 = false) [set short_19_17 0] [set short_19_17 short_19_17 set path19 path19 + 1] ]
  ask node 19 [ifelse (short_19_18 = false) [set short_19_18 0] [set short_19_18 short_19_18 set path19 path19 + 1] ]
  ask node 19 [ifelse (short_19_19 = false) [set short_19_19 0] [set short_19_19 short_19_19] ]
  ask node 19 [ifelse (short_19_20 = false) [set short_19_20 0] [set short_19_20 short_19_20 set path19 path19 + 1] ]
  ask node 19 [ifelse (short_19_21 = false) [set short_19_21 0] [set short_19_21 short_19_21 set path19 path19 + 1] ]
  ask node 19 [ifelse (short_19_22 = false) [set short_19_22 0] [set short_19_22 short_19_22 set path19 path19 + 1] ]
  ask node 19 [ifelse (short_19_23 = false) [set short_19_23 0] [set short_19_23 short_19_23 set path19 path19 + 1] ]
  ask node 19 [ifelse (short_19_24 = false) [set short_19_24 0] [set short_19_24 short_19_24 set path19 path19 + 1] ]
  ask node 19 [ifelse (short_19_25 = false) [set short_19_25 0] [set short_19_25 short_19_25 set path19 path19 + 1] ]
  ask node 19 [ifelse (short_19_26 = false) [set short_19_26 0] [set short_19_26 short_19_26 set path19 path19 + 1] ]

 ; ask node 19 [show path19] ;path verified ;22 other nodes in the NoF show possible paths with node 19 hence the total paths from node 19 is 22.


;; Finding paths between node 20 and other factors

  ask node 20 [set short_20_0 nw:distance-to node 0]
  ask node 20 [set short_20_1 nw:distance-to node 1]
  ask node 20 [set short_20_2 nw:distance-to node 2]
  ask node 20 [set short_20_3 nw:distance-to node 3]
  ask node 20 [set short_20_4 nw:distance-to node 4]
  ask node 20 [set short_20_5 nw:distance-to node 5]
  ask node 20 [set short_20_6 nw:distance-to node 6]
  ask node 20 [set short_20_7 nw:distance-to node 7]
  ask node 20 [set short_20_8 nw:distance-to node 8]
  ask node 20 [set short_20_9 nw:distance-to node 9]
  ask node 20 [set short_20_10 nw:distance-to node 10]
  ask node 20 [set short_20_11 nw:distance-to node 11]
  ask node 20 [set short_20_12 nw:distance-to node 12]
  ask node 20 [set short_20_13 nw:distance-to node 13]
  ask node 20 [set short_20_14 nw:distance-to node 14]
  ask node 20 [set short_20_15 nw:distance-to node 15]
  ask node 20 [set short_20_16 nw:distance-to node 16]
  ask node 20 [set short_20_17 nw:distance-to node 17]
  ask node 20 [set short_20_18 nw:distance-to node 18]
  ask node 20 [set short_20_19 nw:distance-to node 19]
  ask node 20 [set short_20_20 nw:distance-to node 20]
  ask node 20 [set short_20_21 nw:distance-to node 21]
  ask node 20 [set short_20_22 nw:distance-to node 22]
  ask node 20 [set short_20_23 nw:distance-to node 23]
  ask node 20 [set short_20_24 nw:distance-to node 24]
  ask node 20 [set short_20_25 nw:distance-to node 25]
  ask node 20 [set short_20_26 nw:distance-to node 26]

 ;ask node 20 [show short_20_0 show short_20_1 show short_20_2 show short_20_3 show short_20_4 show short_20_5 show short_20_6 show short_20_7 show short_20_8 show short_20_9 show short_20_10 show short_20_11 show short_20_12 show short_20_13 show short_20_14 show short_20_15 show short_20_16 show short_20_17 show short_20_18 show short_20_19 show short_20_20 show short_20_21 show short_20_22 show short_20_23 show short_20_24 show short_20_25 show short_20_26]

  ask node 20 [ set path20 0 ]
  ask node 20 [ifelse (short_20_0 = false) [set short_20_0 0] [set short_20_0 short_20_0 set path20 path20 + 1] ]
  ask node 20 [ifelse (short_20_1 = false) [set short_20_1 0] [set short_20_1 short_20_1 set path20 path20 + 1] ]
  ask node 20 [ifelse (short_20_2 = false) [set short_20_2 0] [set short_20_2 short_20_2 set path20 path20 + 1] ]
  ask node 20 [ifelse (short_20_3 = false) [set short_20_3 0] [set short_20_3 short_20_3 set path20 path20 + 1] ]
  ask node 20 [ifelse (short_20_4 = false) [set short_20_4 0] [set short_20_4 short_20_4 set path20 path20 + 1] ]
  ask node 20 [ifelse (short_20_5 = false) [set short_20_5 0] [set short_20_5 short_20_5 set path20 path20 + 1] ]
  ask node 20 [ifelse (short_20_6 = false) [set short_20_6 0] [set short_20_6 short_20_6 set path20 path20 + 1] ]
  ask node 20 [ifelse (short_20_7 = false) [set short_20_7 0] [set short_20_7 short_20_7 set path20 path20 + 1] ]
  ask node 20 [ifelse (short_20_8 = false) [set short_20_8 0] [set short_20_8 short_20_8 set path20 path20 + 1] ]
  ask node 20 [ifelse (short_20_9 = false) [set short_20_9 0] [set short_20_9 short_20_9 set path20 path20 + 1] ]
  ask node 20 [ifelse (short_20_10 = false) [set short_20_10 0] [set short_20_10 short_20_10 set path20 path20 + 1] ]
  ask node 20 [ifelse (short_20_11 = false) [set short_20_11 0] [set short_20_11 short_20_11 set path20 path20 + 1] ]
  ask node 20 [ifelse (short_20_12 = false) [set short_20_12 0] [set short_20_12 short_20_12 set path20 path20 + 1] ]
  ask node 20 [ifelse (short_20_13 = false) [set short_20_13 0] [set short_20_13 short_20_13 set path20 path20 + 1] ]
  ask node 20 [ifelse (short_20_14 = false) [set short_20_14 0] [set short_20_14 short_20_14 set path20 path20 + 1] ]
  ask node 20 [ifelse (short_20_15 = false) [set short_20_15 0] [set short_20_15 short_20_15 set path20 path20 + 1] ]
  ask node 20 [ifelse (short_20_16 = false) [set short_20_16 0] [set short_20_16 short_20_16 set path20 path20 + 1] ]
  ask node 20 [ifelse (short_20_17 = false) [set short_20_17 0] [set short_20_17 short_20_17 set path20 path20 + 1] ]
  ask node 20 [ifelse (short_20_18 = false) [set short_20_18 0] [set short_20_18 short_20_18 set path20 path20 + 1] ]
  ask node 20 [ifelse (short_20_19 = false) [set short_20_19 0] [set short_20_19 short_20_19 set path20 path20 + 1] ]
  ask node 20 [ifelse (short_20_20 = false) [set short_20_20 0] [set short_20_20 short_20_20] ]
  ask node 20 [ifelse (short_20_21 = false) [set short_20_21 0] [set short_20_21 short_20_21 set path20 path20 + 1] ]
  ask node 20 [ifelse (short_20_22 = false) [set short_20_22 0] [set short_20_22 short_20_22 set path20 path20 + 1] ]
  ask node 20 [ifelse (short_20_23 = false) [set short_20_23 0] [set short_20_23 short_20_23 set path20 path20 + 1] ]
  ask node 20 [ifelse (short_20_24 = false) [set short_20_24 0] [set short_20_24 short_20_24 set path20 path20 + 1] ]
  ask node 20 [ifelse (short_20_25 = false) [set short_20_25 0] [set short_20_25 short_20_25 set path20 path20 + 1] ]
  ask node 20 [ifelse (short_20_26 = false) [set short_20_26 0] [set short_20_26 short_20_26 set path20 path20 + 1] ]

 ; ask node 20 [show path20] ;path verified ;23 other nodes in the NoF show possible paths with node 20 hence the total paths from node 20 is 23.


;; Finding paths between node 21 and other factors

  ask node 21 [set short_21_0 nw:distance-to node 0]
  ask node 21 [set short_21_1 nw:distance-to node 1]
  ask node 21 [set short_21_2 nw:distance-to node 2]
  ask node 21 [set short_21_3 nw:distance-to node 3]
  ask node 21 [set short_21_4 nw:distance-to node 4]
  ask node 21 [set short_21_5 nw:distance-to node 5]
  ask node 21 [set short_21_6 nw:distance-to node 6]
  ask node 21 [set short_21_7 nw:distance-to node 7]
  ask node 21 [set short_21_8 nw:distance-to node 8]
  ask node 21 [set short_21_9 nw:distance-to node 9]
  ask node 21 [set short_21_10 nw:distance-to node 10]
  ask node 21 [set short_21_11 nw:distance-to node 11]
  ask node 21 [set short_21_12 nw:distance-to node 12]
  ask node 21 [set short_21_13 nw:distance-to node 13]
  ask node 21 [set short_21_14 nw:distance-to node 14]
  ask node 21 [set short_21_15 nw:distance-to node 15]
  ask node 21 [set short_21_16 nw:distance-to node 16]
  ask node 21 [set short_21_17 nw:distance-to node 17]
  ask node 21 [set short_21_18 nw:distance-to node 18]
  ask node 21 [set short_21_19 nw:distance-to node 19]
  ask node 21 [set short_21_20 nw:distance-to node 20]
  ask node 21 [set short_21_21 nw:distance-to node 21]
  ask node 21 [set short_21_22 nw:distance-to node 22]
  ask node 21 [set short_21_23 nw:distance-to node 23]
  ask node 21 [set short_21_24 nw:distance-to node 24]
  ask node 21 [set short_21_25 nw:distance-to node 25]
  ask node 21 [set short_21_26 nw:distance-to node 26]

 ;ask node 21 [show short_21_0 show short_21_1 show short_21_2 show short_21_3 show short_21_4 show short_21_5 show short_21_6 show short_21_7 show short_21_8 show short_21_9 show short_21_10 show short_21_11 show short_21_12 show short_21_13 show short_21_14 show short_21_15 show short_21_16 show short_21_17 show short_21_18 show short_21_19 show short_21_20 show short_21_21 show short_21_22 show short_21_23 show short_21_24 show short_21_25 show short_21_26]

  ask node 21 [ set path21 0 ]
  ask node 21 [ifelse (short_21_0 = false) [set short_21_0 0] [set short_21_0 short_21_0 set path21 path21 + 1] ]
  ask node 21 [ifelse (short_21_1 = false) [set short_21_1 0] [set short_21_1 short_21_1 set path21 path21 + 1] ]
  ask node 21 [ifelse (short_21_2 = false) [set short_21_2 0] [set short_21_2 short_21_2 set path21 path21 + 1] ]
  ask node 21 [ifelse (short_21_3 = false) [set short_21_3 0] [set short_21_3 short_21_3 set path21 path21 + 1] ]
  ask node 21 [ifelse (short_21_4 = false) [set short_21_4 0] [set short_21_4 short_21_4 set path21 path21 + 1] ]
  ask node 21 [ifelse (short_21_5 = false) [set short_21_5 0] [set short_21_5 short_21_5 set path21 path21 + 1] ]
  ask node 21 [ifelse (short_21_6 = false) [set short_21_6 0] [set short_21_6 short_21_6 set path21 path21 + 1] ]
  ask node 21 [ifelse (short_21_7 = false) [set short_21_7 0] [set short_21_7 short_21_7 set path21 path21 + 1] ]
  ask node 21 [ifelse (short_21_8 = false) [set short_21_8 0] [set short_21_8 short_21_8 set path21 path21 + 1] ]
  ask node 21 [ifelse (short_21_9 = false) [set short_21_9 0] [set short_21_9 short_21_9 set path21 path21 + 1] ]
  ask node 21 [ifelse (short_21_10 = false) [set short_21_10 0] [set short_21_10 short_21_10 set path21 path21 + 1] ]
  ask node 21 [ifelse (short_21_11 = false) [set short_21_11 0] [set short_21_11 short_21_11 set path21 path21 + 1] ]
  ask node 21 [ifelse (short_21_12 = false) [set short_21_12 0] [set short_21_12 short_21_12 set path21 path21 + 1] ]
  ask node 21 [ifelse (short_21_13 = false) [set short_21_13 0] [set short_21_13 short_21_13 set path21 path21 + 1] ]
  ask node 21 [ifelse (short_21_14 = false) [set short_21_14 0] [set short_21_14 short_21_14 set path21 path21 + 1] ]
  ask node 21 [ifelse (short_21_15 = false) [set short_21_15 0] [set short_21_15 short_21_15 set path21 path21 + 1] ]
  ask node 21 [ifelse (short_21_16 = false) [set short_21_16 0] [set short_21_16 short_21_16 set path21 path21 + 1] ]
  ask node 21 [ifelse (short_21_17 = false) [set short_21_17 0] [set short_21_17 short_21_17 set path21 path21 + 1] ]
  ask node 21 [ifelse (short_21_18 = false) [set short_21_18 0] [set short_21_18 short_21_18 set path21 path21 + 1] ]
  ask node 21 [ifelse (short_21_19 = false) [set short_21_19 0] [set short_21_19 short_21_19 set path21 path21 + 1] ]
  ask node 21 [ifelse (short_21_20 = false) [set short_21_20 0] [set short_21_20 short_21_20 set path21 path21 + 1] ]
  ask node 21 [ifelse (short_21_21 = false) [set short_21_21 0] [set short_21_21 short_21_21] ]
  ask node 21 [ifelse (short_21_22 = false) [set short_21_22 0] [set short_21_22 short_21_22 set path21 path21 + 1] ]
  ask node 21 [ifelse (short_21_23 = false) [set short_21_23 0] [set short_21_23 short_21_23 set path21 path21 + 1] ]
  ask node 21 [ifelse (short_21_24 = false) [set short_21_24 0] [set short_21_24 short_21_24 set path21 path21 + 1] ]
  ask node 21 [ifelse (short_21_25 = false) [set short_21_25 0] [set short_21_25 short_21_25 set path21 path21 + 1] ]
  ask node 21 [ifelse (short_21_26 = false) [set short_21_26 0] [set short_21_26 short_21_26 set path21 path21 + 1] ]

  ;ask node 21 [show path21] ;path verified ;17 other nodes in the NoF show possible paths with node 21 hence the total paths from node 21 is 17.


;; Finding paths between node 22 and other factors

  ask node 22 [set short_22_0 nw:distance-to node 0]
  ask node 22 [set short_22_1 nw:distance-to node 1]
  ask node 22 [set short_22_2 nw:distance-to node 2]
  ask node 22 [set short_22_3 nw:distance-to node 3]
  ask node 22 [set short_22_4 nw:distance-to node 4]
  ask node 22 [set short_22_5 nw:distance-to node 5]
  ask node 22 [set short_22_6 nw:distance-to node 6]
  ask node 22 [set short_22_7 nw:distance-to node 7]
  ask node 22 [set short_22_8 nw:distance-to node 8]
  ask node 22 [set short_22_9 nw:distance-to node 9]
  ask node 22 [set short_22_10 nw:distance-to node 10]
  ask node 22 [set short_22_11 nw:distance-to node 11]
  ask node 22 [set short_22_12 nw:distance-to node 12]
  ask node 22 [set short_22_13 nw:distance-to node 13]
  ask node 22 [set short_22_14 nw:distance-to node 14]
  ask node 22 [set short_22_15 nw:distance-to node 15]
  ask node 22 [set short_22_16 nw:distance-to node 16]
  ask node 22 [set short_22_17 nw:distance-to node 17]
  ask node 22 [set short_22_18 nw:distance-to node 18]
  ask node 22 [set short_22_19 nw:distance-to node 19]
  ask node 22 [set short_22_20 nw:distance-to node 20]
  ask node 22 [set short_22_21 nw:distance-to node 21]
  ask node 22 [set short_22_22 nw:distance-to node 22]
  ask node 22 [set short_22_23 nw:distance-to node 23]
  ask node 22 [set short_22_24 nw:distance-to node 24]
  ask node 22 [set short_22_25 nw:distance-to node 25]
  ask node 22 [set short_22_26 nw:distance-to node 26]

  ;ask node 22 [show short_22_0 show short_22_1 show short_22_2 show short_22_3 show short_22_4 show short_22_5 show short_22_6 show short_22_7 show short_22_8 show short_22_9 show short_22_10 show short_22_11 show short_22_12 show short_22_13 show short_22_14 show short_22_15 show short_22_16 show short_22_17 show short_22_18 show short_22_19 show short_22_20 show short_22_21 show short_22_22 show short_22_23 show short_22_24 show short_22_25 show short_22_26]

  ask node 22 [ set path22 0 ]
  ask node 22 [ifelse (short_22_0 = false) [set short_22_0 0] [set short_22_0 short_22_0 set path22 path22 + 1] ]
  ask node 22 [ifelse (short_22_1 = false) [set short_22_1 0] [set short_22_1 short_22_1 set path22 path22 + 1] ]
  ask node 22 [ifelse (short_22_2 = false) [set short_22_2 0] [set short_22_2 short_22_2 set path22 path22 + 1] ]
  ask node 22 [ifelse (short_22_3 = false) [set short_22_3 0] [set short_22_3 short_22_3 set path22 path22 + 1] ]
  ask node 22 [ifelse (short_22_4 = false) [set short_22_4 0] [set short_22_4 short_22_4 set path22 path22 + 1] ]
  ask node 22 [ifelse (short_22_5 = false) [set short_22_5 0] [set short_22_5 short_22_5 set path22 path22 + 1] ]
  ask node 22 [ifelse (short_22_6 = false) [set short_22_6 0] [set short_22_6 short_22_6 set path22 path22 + 1] ]
  ask node 22 [ifelse (short_22_7 = false) [set short_22_7 0] [set short_22_7 short_22_7 set path22 path22 + 1] ]
  ask node 22 [ifelse (short_22_8 = false) [set short_22_8 0] [set short_22_8 short_22_8 set path22 path22 + 1] ]
  ask node 22 [ifelse (short_22_9 = false) [set short_22_9 0] [set short_22_9 short_22_9 set path22 path22 + 1] ]
  ask node 22 [ifelse (short_22_10 = false) [set short_22_10 0] [set short_22_10 short_22_10 set path22 path22 + 1] ]
  ask node 22 [ifelse (short_22_11 = false) [set short_22_11 0] [set short_22_11 short_22_11 set path22 path22 + 1] ]
  ask node 22 [ifelse (short_22_12 = false) [set short_22_12 0] [set short_22_12 short_22_12 set path22 path22 + 1] ]
  ask node 22 [ifelse (short_22_13 = false) [set short_22_13 0] [set short_22_13 short_22_13 set path22 path22 + 1] ]
  ask node 22 [ifelse (short_22_14 = false) [set short_22_14 0] [set short_22_14 short_22_14 set path22 path22 + 1] ]
  ask node 22 [ifelse (short_22_15 = false) [set short_22_15 0] [set short_22_15 short_22_15 set path22 path22 + 1] ]
  ask node 22 [ifelse (short_22_16 = false) [set short_22_16 0] [set short_22_16 short_22_16 set path22 path22 + 1] ]
  ask node 22 [ifelse (short_22_17 = false) [set short_22_17 0] [set short_22_17 short_22_17 set path22 path22 + 1] ]
  ask node 22 [ifelse (short_22_18 = false) [set short_22_18 0] [set short_22_18 short_22_18 set path22 path22 + 1] ]
  ask node 22 [ifelse (short_22_19 = false) [set short_22_19 0] [set short_22_19 short_22_19 set path22 path22 + 1] ]
  ask node 22 [ifelse (short_22_20 = false) [set short_22_20 0] [set short_22_20 short_22_20 set path22 path22 + 1] ]
  ask node 22 [ifelse (short_22_21 = false) [set short_22_21 0] [set short_22_21 short_22_21 set path22 path22 + 1] ]
  ask node 22 [ifelse (short_22_22 = false) [set short_22_22 0] [set short_22_22 short_22_22] ]
  ask node 22 [ifelse (short_22_23 = false) [set short_22_23 0] [set short_22_23 short_22_23 set path22 path22 + 1] ]
  ask node 22 [ifelse (short_22_24 = false) [set short_22_24 0] [set short_22_24 short_22_24 set path22 path22 + 1] ]
  ask node 22 [ifelse (short_22_25 = false) [set short_22_25 0] [set short_22_25 short_22_25 set path22 path22 + 1] ]
  ask node 22 [ifelse (short_22_26 = false) [set short_22_26 0] [set short_22_26 short_22_26 set path22 path22 + 1] ]

  ;ask node 22 [show path22] ;path verified ;22 other nodes in the NoF show possible paths with node 22 hence the total paths from node 22 is 22.


;; Finding paths between node 23 and other factors

  ask node 23 [set short_23_0 nw:distance-to node 0]
  ask node 23 [set short_23_1 nw:distance-to node 1]
  ask node 23 [set short_23_2 nw:distance-to node 2]
  ask node 23 [set short_23_3 nw:distance-to node 3]
  ask node 23 [set short_23_4 nw:distance-to node 4]
  ask node 23 [set short_23_5 nw:distance-to node 5]
  ask node 23 [set short_23_6 nw:distance-to node 6]
  ask node 23 [set short_23_7 nw:distance-to node 7]
  ask node 23 [set short_23_8 nw:distance-to node 8]
  ask node 23 [set short_23_9 nw:distance-to node 9]
  ask node 23 [set short_23_10 nw:distance-to node 10]
  ask node 23 [set short_23_11 nw:distance-to node 11]
  ask node 23 [set short_23_12 nw:distance-to node 12]
  ask node 23 [set short_23_13 nw:distance-to node 13]
  ask node 23 [set short_23_14 nw:distance-to node 14]
  ask node 23 [set short_23_15 nw:distance-to node 15]
  ask node 23 [set short_23_16 nw:distance-to node 16]
  ask node 23 [set short_23_17 nw:distance-to node 17]
  ask node 23 [set short_23_18 nw:distance-to node 18]
  ask node 23 [set short_23_19 nw:distance-to node 19]
  ask node 23 [set short_23_20 nw:distance-to node 20]
  ask node 23 [set short_23_21 nw:distance-to node 21]
  ask node 23 [set short_23_22 nw:distance-to node 22]
  ask node 23 [set short_23_23 nw:distance-to node 23]
  ask node 23 [set short_23_24 nw:distance-to node 24]
  ask node 23 [set short_23_25 nw:distance-to node 25]
  ask node 23 [set short_23_26 nw:distance-to node 26]

  ;ask node 23 [show short_23_0 show short_23_1 show short_23_2 show short_23_3 show short_23_4 show short_23_5 show short_23_6 show short_23_7 show short_23_8 show short_23_9 show short_23_10 show short_23_11 show short_23_12 show short_23_13 show short_23_14 show short_23_15 show short_23_16 show short_23_17 show short_23_18 show short_23_19 show short_23_20 show short_23_21 show short_23_22 show short_23_23 show short_23_24 show short_23_25 show short_23_26]

  ask node 23 [ set path23 0 ]
  ask node 23 [ifelse (short_23_0 = false) [set short_23_0 0] [set short_23_0 short_23_0 set path23 path23 + 1] ]
  ask node 23 [ifelse (short_23_1 = false) [set short_23_1 0] [set short_23_1 short_23_1 set path23 path23 + 1] ]
  ask node 23 [ifelse (short_23_2 = false) [set short_23_2 0] [set short_23_2 short_23_2 set path23 path23 + 1] ]
  ask node 23 [ifelse (short_23_3 = false) [set short_23_3 0] [set short_23_3 short_23_3 set path23 path23 + 1] ]
  ask node 23 [ifelse (short_23_4 = false) [set short_23_4 0] [set short_23_4 short_23_4 set path23 path23 + 1] ]
  ask node 23 [ifelse (short_23_5 = false) [set short_23_5 0] [set short_23_5 short_23_5 set path23 path23 + 1] ]
  ask node 23 [ifelse (short_23_6 = false) [set short_23_6 0] [set short_23_6 short_23_6 set path23 path23 + 1] ]
  ask node 23 [ifelse (short_23_7 = false) [set short_23_7 0] [set short_23_7 short_23_7 set path23 path23 + 1] ]
  ask node 23 [ifelse (short_23_8 = false) [set short_23_8 0] [set short_23_8 short_23_8 set path23 path23 + 1] ]
  ask node 23 [ifelse (short_23_9 = false) [set short_23_9 0] [set short_23_9 short_23_9 set path23 path23 + 1] ]
  ask node 23 [ifelse (short_23_10 = false) [set short_23_10 0] [set short_23_10 short_23_10 set path23 path23 + 1] ]
  ask node 23 [ifelse (short_23_11 = false) [set short_23_11 0] [set short_23_11 short_23_11 set path23 path23 + 1] ]
  ask node 23 [ifelse (short_23_12 = false) [set short_23_12 0] [set short_23_12 short_23_12 set path23 path23 + 1] ]
  ask node 23 [ifelse (short_23_13 = false) [set short_23_13 0] [set short_23_13 short_23_13 set path23 path23 + 1] ]
  ask node 23 [ifelse (short_23_14 = false) [set short_23_14 0] [set short_23_14 short_23_14 set path23 path23 + 1] ]
  ask node 23 [ifelse (short_23_15 = false) [set short_23_15 0] [set short_23_15 short_23_15 set path23 path23 + 1] ]
  ask node 23 [ifelse (short_23_16 = false) [set short_23_16 0] [set short_23_16 short_23_16 set path23 path23 + 1] ]
  ask node 23 [ifelse (short_23_17 = false) [set short_23_17 0] [set short_23_17 short_23_17 set path23 path23 + 1] ]
  ask node 23 [ifelse (short_23_18 = false) [set short_23_18 0] [set short_23_18 short_23_18 set path23 path23 + 1] ]
  ask node 23 [ifelse (short_23_19 = false) [set short_23_19 0] [set short_23_19 short_23_19 set path23 path23 + 1] ]
  ask node 23 [ifelse (short_23_20 = false) [set short_23_20 0] [set short_23_20 short_23_20 set path23 path23 + 1] ]
  ask node 23 [ifelse (short_23_21 = false) [set short_23_21 0] [set short_23_21 short_23_21 set path23 path23 + 1] ]
  ask node 23 [ifelse (short_23_22 = false) [set short_23_22 0] [set short_23_22 short_23_22 set path23 path23 + 1] ]
  ask node 23 [ifelse (short_23_23 = false) [set short_23_23 0] [set short_23_23 short_23_23] ]
  ask node 23 [ifelse (short_23_24 = false) [set short_23_24 0] [set short_23_24 short_23_24 set path23 path23 + 1] ]
  ask node 23 [ifelse (short_23_25 = false) [set short_23_25 0] [set short_23_25 short_23_25 set path23 path23 + 1] ]
  ask node 23 [ifelse (short_23_26 = false) [set short_23_26 0] [set short_23_26 short_23_26 set path23 path23 + 1] ]

  ;ask node 23 [show path23] ;path verified ;22 other nodes in the NoF show possible paths with node 23 hence the total paths from node 23 is 22.



;; Finding paths between node 24 and other factors

  ask node 24 [set short_24_0 nw:distance-to node 0]
  ask node 24 [set short_24_1 nw:distance-to node 1]
  ask node 24 [set short_24_2 nw:distance-to node 2]
  ask node 24 [set short_24_3 nw:distance-to node 3]
  ask node 24 [set short_24_4 nw:distance-to node 4]
  ask node 24 [set short_24_5 nw:distance-to node 5]
  ask node 24 [set short_24_6 nw:distance-to node 6]
  ask node 24 [set short_24_7 nw:distance-to node 7]
  ask node 24 [set short_24_8 nw:distance-to node 8]
  ask node 24 [set short_24_9 nw:distance-to node 9]
  ask node 24 [set short_24_10 nw:distance-to node 10]
  ask node 24 [set short_24_11 nw:distance-to node 11]
  ask node 24 [set short_24_12 nw:distance-to node 12]
  ask node 24 [set short_24_13 nw:distance-to node 13]
  ask node 24 [set short_24_14 nw:distance-to node 14]
  ask node 24 [set short_24_15 nw:distance-to node 15]
  ask node 24 [set short_24_16 nw:distance-to node 16]
  ask node 24 [set short_24_17 nw:distance-to node 17]
  ask node 24 [set short_24_18 nw:distance-to node 18]
  ask node 24 [set short_24_19 nw:distance-to node 19]
  ask node 24 [set short_24_20 nw:distance-to node 20]
  ask node 24 [set short_24_21 nw:distance-to node 21]
  ask node 24 [set short_24_22 nw:distance-to node 22]
  ask node 24 [set short_24_23 nw:distance-to node 23]
  ask node 24 [set short_24_24 nw:distance-to node 24]
  ask node 24 [set short_24_25 nw:distance-to node 25]
  ask node 24 [set short_24_26 nw:distance-to node 26]

  ;ask node 24 [show short_24_0 show short_24_1 show short_24_2 show short_24_3 show short_24_4 show short_24_5 show short_24_6 show short_24_7 show short_24_8 show short_24_9 show short_24_10 show short_24_11 show short_24_12 show short_24_13 show short_24_14 show short_24_15 show short_24_16 show short_24_17 show short_24_18 show short_24_19 show short_24_20 show short_24_21 show short_24_22 show short_24_23 show short_24_24 show short_24_25 show short_24_26]

  ask node 24 [ set path24 0 ]
  ask node 24 [ifelse (short_24_0 = false) [set short_24_0 0] [set short_24_0 short_24_0 set path24 path24 + 1] ]
  ask node 24 [ifelse (short_24_1 = false) [set short_24_1 0] [set short_24_1 short_24_1 set path24 path24 + 1] ]
  ask node 24 [ifelse (short_24_2 = false) [set short_24_2 0] [set short_24_2 short_24_2 set path24 path24 + 1] ]
  ask node 24 [ifelse (short_24_3 = false) [set short_24_3 0] [set short_24_3 short_24_3 set path24 path24 + 1] ]
  ask node 24 [ifelse (short_24_4 = false) [set short_24_4 0] [set short_24_4 short_24_4 set path24 path24 + 1] ]
  ask node 24 [ifelse (short_24_5 = false) [set short_24_5 0] [set short_24_5 short_24_5 set path24 path24 + 1] ]
  ask node 24 [ifelse (short_24_6 = false) [set short_24_6 0] [set short_24_6 short_24_6 set path24 path24 + 1] ]
  ask node 24 [ifelse (short_24_7 = false) [set short_24_7 0] [set short_24_7 short_24_7 set path24 path24 + 1] ]
  ask node 24 [ifelse (short_24_8 = false) [set short_24_8 0] [set short_24_8 short_24_8 set path24 path24 + 1] ]
  ask node 24 [ifelse (short_24_9 = false) [set short_24_9 0] [set short_24_9 short_24_9 set path24 path24 + 1] ]
  ask node 24 [ifelse (short_24_10 = false) [set short_24_10 0] [set short_24_10 short_24_10 set path24 path24 + 1] ]
  ask node 24 [ifelse (short_24_11 = false) [set short_24_11 0] [set short_24_11 short_24_11 set path24 path24 + 1] ]
  ask node 24 [ifelse (short_24_12 = false) [set short_24_12 0] [set short_24_12 short_24_12 set path24 path24 + 1] ]
  ask node 24 [ifelse (short_24_13 = false) [set short_24_13 0] [set short_24_13 short_24_13 set path24 path24 + 1] ]
  ask node 24 [ifelse (short_24_14 = false) [set short_24_14 0] [set short_24_14 short_24_14 set path24 path24 + 1] ]
  ask node 24 [ifelse (short_24_15 = false) [set short_24_15 0] [set short_24_15 short_24_15 set path24 path24 + 1] ]
  ask node 24 [ifelse (short_24_16 = false) [set short_24_16 0] [set short_24_16 short_24_16 set path24 path24 + 1] ]
  ask node 24 [ifelse (short_24_17 = false) [set short_24_17 0] [set short_24_17 short_24_17 set path24 path24 + 1] ]
  ask node 24 [ifelse (short_24_18 = false) [set short_24_18 0] [set short_24_18 short_24_18 set path24 path24 + 1] ]
  ask node 24 [ifelse (short_24_19 = false) [set short_24_19 0] [set short_24_19 short_24_19 set path24 path24 + 1] ]
  ask node 24 [ifelse (short_24_20 = false) [set short_24_20 0] [set short_24_20 short_24_20 set path24 path24 + 1] ]
  ask node 24 [ifelse (short_24_21 = false) [set short_24_21 0] [set short_24_21 short_24_21 set path24 path24 + 1] ]
  ask node 24 [ifelse (short_24_22 = false) [set short_24_22 0] [set short_24_22 short_24_22 set path24 path24 + 1] ]
  ask node 24 [ifelse (short_24_23 = false) [set short_24_23 0] [set short_24_23 short_24_23 set path24 path24 + 1] ]
  ask node 24 [ifelse (short_24_24 = false) [set short_24_24 0] [set short_24_24 short_24_24] ]
  ask node 24 [ifelse (short_24_25 = false) [set short_24_25 0] [set short_24_25 short_24_25 set path24 path24 + 1] ]
  ask node 24 [ifelse (short_24_26 = false) [set short_24_26 0] [set short_24_26 short_24_26 set path24 path24 + 1] ]

  ;ask node 24 [show path24] ;path verified ;22 other nodes in the NoF show possible paths with node 24 hence the total paths from node 24 is 22.



;; Finding paths between node 25 and other factors

  ask node 25 [set short_25_0 nw:distance-to node 0]
  ask node 25 [set short_25_1 nw:distance-to node 1]
  ask node 25 [set short_25_2 nw:distance-to node 2]
  ask node 25 [set short_25_3 nw:distance-to node 3]
  ask node 25 [set short_25_4 nw:distance-to node 4]
  ask node 25 [set short_25_5 nw:distance-to node 5]
  ask node 25 [set short_25_6 nw:distance-to node 6]
  ask node 25 [set short_25_7 nw:distance-to node 7]
  ask node 25 [set short_25_8 nw:distance-to node 8]
  ask node 25 [set short_25_9 nw:distance-to node 9]
  ask node 25 [set short_25_10 nw:distance-to node 10]
  ask node 25 [set short_25_11 nw:distance-to node 11]
  ask node 25 [set short_25_12 nw:distance-to node 12]
  ask node 25 [set short_25_13 nw:distance-to node 13]
  ask node 25 [set short_25_14 nw:distance-to node 14]
  ask node 25 [set short_25_15 nw:distance-to node 15]
  ask node 25 [set short_25_16 nw:distance-to node 16]
  ask node 25 [set short_25_17 nw:distance-to node 17]
  ask node 25 [set short_25_18 nw:distance-to node 18]
  ask node 25 [set short_25_19 nw:distance-to node 19]
  ask node 25 [set short_25_20 nw:distance-to node 20]
  ask node 25 [set short_25_21 nw:distance-to node 21]
  ask node 25 [set short_25_22 nw:distance-to node 22]
  ask node 25 [set short_25_23 nw:distance-to node 23]
  ask node 25 [set short_25_24 nw:distance-to node 24]
  ask node 25 [set short_25_25 nw:distance-to node 25]
  ask node 25 [set short_25_26 nw:distance-to node 26]

  ;ask node 25 [show short_25_0 show short_25_1 show short_25_2 show short_25_3 show short_25_4 show short_25_5 show short_25_6 show short_25_7 show short_25_8 show short_25_9 show short_25_10 show short_25_11 show short_25_12 show short_25_13 show short_25_14 show short_25_15 show short_25_16 show short_25_17 show short_25_18 show short_25_19 show short_25_20 show short_25_21 show short_25_22 show short_25_23 show short_25_24 show short_25_25 show short_25_26]

  ask node 25 [ set path25 0 ]
  ask node 25 [ifelse (short_25_0 = false) [set short_25_0 0] [set short_25_0 short_25_0 set path25 path25 + 1] ]
  ask node 25 [ifelse (short_25_1 = false) [set short_25_1 0] [set short_25_1 short_25_1 set path25 path25 + 1] ]
  ask node 25 [ifelse (short_25_2 = false) [set short_25_2 0] [set short_25_2 short_25_2 set path25 path25 + 1] ]
  ask node 25 [ifelse (short_25_3 = false) [set short_25_3 0] [set short_25_3 short_25_3 set path25 path25 + 1] ]
  ask node 25 [ifelse (short_25_4 = false) [set short_25_4 0] [set short_25_4 short_25_4 set path25 path25 + 1] ]
  ask node 25 [ifelse (short_25_5 = false) [set short_25_5 0] [set short_25_5 short_25_5 set path25 path25 + 1] ]
  ask node 25 [ifelse (short_25_6 = false) [set short_25_6 0] [set short_25_6 short_25_6 set path25 path25 + 1] ]
  ask node 25 [ifelse (short_25_7 = false) [set short_25_7 0] [set short_25_7 short_25_7 set path25 path25 + 1] ]
  ask node 25 [ifelse (short_25_8 = false) [set short_25_8 0] [set short_25_8 short_25_8 set path25 path25 + 1] ]
  ask node 25 [ifelse (short_25_9 = false) [set short_25_9 0] [set short_25_9 short_25_9 set path25 path25 + 1] ]
  ask node 25 [ifelse (short_25_10 = false) [set short_25_10 0] [set short_25_10 short_25_10 set path25 path25 + 1] ]
  ask node 25 [ifelse (short_25_11 = false) [set short_25_11 0] [set short_25_11 short_25_11 set path25 path25 + 1] ]
  ask node 25 [ifelse (short_25_12 = false) [set short_25_12 0] [set short_25_12 short_25_12 set path25 path25 + 1] ]
  ask node 25 [ifelse (short_25_13 = false) [set short_25_13 0] [set short_25_13 short_25_13 set path25 path25 + 1] ]
  ask node 25 [ifelse (short_25_14 = false) [set short_25_14 0] [set short_25_14 short_25_14 set path25 path25 + 1] ]
  ask node 25 [ifelse (short_25_15 = false) [set short_25_15 0] [set short_25_15 short_25_15 set path25 path25 + 1] ]
  ask node 25 [ifelse (short_25_16 = false) [set short_25_16 0] [set short_25_16 short_25_16 set path25 path25 + 1] ]
  ask node 25 [ifelse (short_25_17 = false) [set short_25_17 0] [set short_25_17 short_25_17 set path25 path25 + 1] ]
  ask node 25 [ifelse (short_25_18 = false) [set short_25_18 0] [set short_25_18 short_25_18 set path25 path25 + 1] ]
  ask node 25 [ifelse (short_25_19 = false) [set short_25_19 0] [set short_25_19 short_25_19 set path25 path25 + 1] ]
  ask node 25 [ifelse (short_25_20 = false) [set short_25_20 0] [set short_25_20 short_25_20 set path25 path25 + 1] ]
  ask node 25 [ifelse (short_25_21 = false) [set short_25_21 0] [set short_25_21 short_25_21 set path25 path25 + 1] ]
  ask node 25 [ifelse (short_25_22 = false) [set short_25_22 0] [set short_25_22 short_25_22 set path25 path25 + 1] ]
  ask node 25 [ifelse (short_25_23 = false) [set short_25_23 0] [set short_25_23 short_25_23 set path25 path25 + 1] ]
  ask node 25 [ifelse (short_25_24 = false) [set short_25_24 0] [set short_25_24 short_25_24 set path25 path25 + 1] ]
  ask node 25 [ifelse (short_25_25 = false) [set short_25_25 0] [set short_25_25 short_25_25] ]
  ask node 25 [ifelse (short_25_26 = false) [set short_25_26 0] [set short_25_26 short_25_26 set path25 path25 + 1] ]

  ;ask node 25 [show path25] ;path verified ;23 other nodes in the NoF show possible paths with node 25 hence the total paths from node 25 is 23.



;; Finding paths between node 26 and other factors

  ask node 26 [set short_26_0 nw:distance-to node 0]
  ask node 26 [set short_26_1 nw:distance-to node 1]
  ask node 26 [set short_26_2 nw:distance-to node 2]
  ask node 26 [set short_26_3 nw:distance-to node 3]
  ask node 26 [set short_26_4 nw:distance-to node 4]
  ask node 26 [set short_26_5 nw:distance-to node 5]
  ask node 26 [set short_26_6 nw:distance-to node 6]
  ask node 26 [set short_26_7 nw:distance-to node 7]
  ask node 26 [set short_26_8 nw:distance-to node 8]
  ask node 26 [set short_26_9 nw:distance-to node 9]
  ask node 26 [set short_26_10 nw:distance-to node 10]
  ask node 26 [set short_26_11 nw:distance-to node 11]
  ask node 26 [set short_26_12 nw:distance-to node 12]
  ask node 26 [set short_26_13 nw:distance-to node 13]
  ask node 26 [set short_26_14 nw:distance-to node 14]
  ask node 26 [set short_26_15 nw:distance-to node 15]
  ask node 26 [set short_26_16 nw:distance-to node 16]
  ask node 26 [set short_26_17 nw:distance-to node 17]
  ask node 26 [set short_26_18 nw:distance-to node 18]
  ask node 26 [set short_26_19 nw:distance-to node 19]
  ask node 26 [set short_26_20 nw:distance-to node 20]
  ask node 26 [set short_26_21 nw:distance-to node 21]
  ask node 26 [set short_26_22 nw:distance-to node 22]
  ask node 26 [set short_26_23 nw:distance-to node 23]
  ask node 26 [set short_26_24 nw:distance-to node 24]
  ask node 26 [set short_26_25 nw:distance-to node 25]
  ask node 26 [set short_26_26 nw:distance-to node 26]

  ;ask node 26 [show short_26_0 show short_26_1 show short_26_2 show short_26_3 show short_26_4 show short_26_5 show short_26_6 show short_26_7 show short_26_8 show short_26_9 show short_26_10 show short_26_11 show short_26_12 show short_26_13 show short_26_14 show short_26_15 show short_26_16 show short_26_17 show short_26_18 show short_26_19 show short_26_20 show short_26_21 show short_26_22 show short_26_23 show short_26_24 show short_26_25 show short_26_26]

  ask node 26 [ set path26 0 ]
  ask node 26 [ifelse (short_26_0 = false) [set short_26_0 0] [set short_26_0 short_26_0 set path26 path26 + 1] ]
  ask node 26 [ifelse (short_26_1 = false) [set short_26_1 0] [set short_26_1 short_26_1 set path26 path26 + 1] ]
  ask node 26 [ifelse (short_26_2 = false) [set short_26_2 0] [set short_26_2 short_26_2 set path26 path26 + 1] ]
  ask node 26 [ifelse (short_26_3 = false) [set short_26_3 0] [set short_26_3 short_26_3 set path26 path26 + 1] ]
  ask node 26 [ifelse (short_26_4 = false) [set short_26_4 0] [set short_26_4 short_26_4 set path26 path26 + 1] ]
  ask node 26 [ifelse (short_26_5 = false) [set short_26_5 0] [set short_26_5 short_26_5 set path26 path26 + 1] ]
  ask node 26 [ifelse (short_26_6 = false) [set short_26_6 0] [set short_26_6 short_26_6 set path26 path26 + 1] ]
  ask node 26 [ifelse (short_26_7 = false) [set short_26_7 0] [set short_26_7 short_26_7 set path26 path26 + 1] ]
  ask node 26 [ifelse (short_26_8 = false) [set short_26_8 0] [set short_26_8 short_26_8 set path26 path26 + 1] ]
  ask node 26 [ifelse (short_26_9 = false) [set short_26_9 0] [set short_26_9 short_26_9 set path26 path26 + 1] ]
  ask node 26 [ifelse (short_26_10 = false) [set short_26_10 0] [set short_26_10 short_26_10 set path26 path26 + 1] ]
  ask node 26 [ifelse (short_26_11 = false) [set short_26_11 0] [set short_26_11 short_26_11 set path26 path26 + 1] ]
  ask node 26 [ifelse (short_26_12 = false) [set short_26_12 0] [set short_26_12 short_26_12 set path26 path26 + 1] ]
  ask node 26 [ifelse (short_26_13 = false) [set short_26_13 0] [set short_26_13 short_26_13 set path26 path26 + 1] ]
  ask node 26 [ifelse (short_26_14 = false) [set short_26_14 0] [set short_26_14 short_26_14 set path26 path26 + 1] ]
  ask node 26 [ifelse (short_26_15 = false) [set short_26_15 0] [set short_26_15 short_26_15 set path26 path26 + 1] ]
  ask node 26 [ifelse (short_26_16 = false) [set short_26_16 0] [set short_26_16 short_26_16 set path26 path26 + 1] ]
  ask node 26 [ifelse (short_26_17 = false) [set short_26_17 0] [set short_26_17 short_26_17 set path26 path26 + 1] ]
  ask node 26 [ifelse (short_26_18 = false) [set short_26_18 0] [set short_26_18 short_26_18 set path26 path26 + 1] ]
  ask node 26 [ifelse (short_26_19 = false) [set short_26_19 0] [set short_26_19 short_26_19 set path26 path26 + 1] ]
  ask node 26 [ifelse (short_26_20 = false) [set short_26_20 0] [set short_26_20 short_26_20 set path26 path26 + 1] ]
  ask node 26 [ifelse (short_26_21 = false) [set short_26_21 0] [set short_26_21 short_26_21 set path26 path26 + 1] ]
  ask node 26 [ifelse (short_26_22 = false) [set short_26_22 0] [set short_26_22 short_26_22 set path26 path26 + 1] ]
  ask node 26 [ifelse (short_26_23 = false) [set short_26_23 0] [set short_26_23 short_26_23 set path26 path26 + 1] ]
  ask node 26 [ifelse (short_26_24 = false) [set short_26_24 0] [set short_26_24 short_26_24 set path26 path26 + 1] ]
  ask node 26 [ifelse (short_26_25 = false) [set short_26_25 0] [set short_26_25 short_26_25 set path26 path26 + 1] ]
  ask node 26 [ifelse (short_26_26 = false) [set short_26_26 0] [set short_26_26 short_26_26] ]

  ;ask node 26 [show path26] ;path verified ;23 other nodes in the NoF show possible paths with node 26 hence the total paths from node 26 is 23.


;; Comment on the procedure: nw:distance-to syntax provides the shortest pathlengths between two nodes.So far we have calculated the pathlength between any two pair of nodes in the network and the possible number of characteristic
  ;pathlengths that can be formed by a node (as indicated by pathi). The pathlength between any two pair of nodes is calculated directly for most nodes
  ; and indirectly for few nodes (i.e., nodes 0, 1, 19, 20, 21, 22, 23, 24, 25, 26). Inorder to get the total of the shortest pathlengths between all nodes we need the summation of all the shortest pathlengths between every pair of nodes in the network.


;; code for calculating the characteristic pathlength of the network ;;

;; First, calculate the total shortest pathlength for every node with other nodes in the network.

  ask node 0 [set short_i short_0_0 + short_0_1 + short_0_2 + short_0_3 + short_0_4 + short_0_5 + short_0_6 + short_0_7 + short_0_8 + short_0_9 + short_0_10 + short_0_11 + short_0_12 + short_0_13 + short_0_14 + short_0_15 + short_0_16 + short_0_17 + short_0_18 + short_0_19 + short_0_20 + short_0_21 + short_0_22 + short_0_23 + short_0_24 + short_0_25 + short_0_26]
  ask node 1 [set short_TR short_1_0 + short_1_1 + short_1_2 + short_1_3 + short_1_4 + short_1_5 + short_1_6 + short_1_7 + short_1_8 + short_1_9 + short_1_10 + short_1_11 + short_1_12 + short_1_13 + short_1_14 + short_1_15 + short_1_16 + short_1_17 + short_1_18 + short_1_19 + short_1_20 + short_1_21 + short_1_22 + short_1_23 + short_1_24 + short_1_25 + short_1_26]
  ask node 2 [set short_R sum[short_2] of nodes]
  ask node 3 [set short_F sum[short_3] of nodes]
  ask node 4 [set short_T sum[short_4] of nodes]
  ask node 5 [set short_n sum[short_5] of nodes]
  ask node 6 [set short_S sum[short_6] of nodes]
  ask node 7 [set short_Cp sum[short_7] of nodes]
  ask node 8 [set short_pHg sum[short_8] of nodes]
  ask node 9 [set short_Xg sum[short_9] of nodes]
  ask node 10 [set short_Cc sum[short_10] of nodes]
  ask node 11 [set short_foc sum[short_11] of nodes]
  ask node 12 [set short_pHw sum[short_12] of nodes]
  ask node 13 [set short_Tw sum[short_13] of nodes]
  ask node 14 [set short_pw sum[short_14] of nodes]
  ask node 15 [set short_Ew sum[short_15] of nodes]
  ask node 16 [set short_Iw sum[short_16] of nodes]
  ask node 17 [set short_Aw sum[short_17] of nodes]
  ask node 18 [set short_DOC sum[short_18] of nodes]
  ask node 19 [set short_pHm short_19_0 + short_19_1 + short_19_2 + short_19_3 + short_19_4 + short_19_5 + short_19_6 + short_19_7 + short_19_8 + short_19_9 + short_19_10 + short_19_11 + short_19_12 + short_19_13 + short_19_14 + short_19_15 + short_19_16 + short_19_17 + short_19_18 + short_19_19 + short_19_20 + short_19_21 + short_19_22 + short_19_23 + short_19_24 + short_19_25 + short_19_26]
  ask node 20 [set short_Tm short_20_0 + short_20_1 + short_20_2 + short_20_3 + short_20_4 + short_20_5 + short_20_6 + short_20_7 + short_20_8 + short_20_9 + short_20_10 + short_20_11 + short_20_12 + short_20_13 + short_20_14 + short_20_15 + short_20_16 + short_20_17 + short_20_18 + short_20_19 + short_20_20 + short_20_21 + short_20_22 + short_20_23 + short_20_24 + short_20_25 + short_20_26]
  ask node 21 [set short_pm short_21_0 + short_21_1 + short_21_2 + short_21_3 + short_21_4 + short_21_5 + short_21_6 + short_21_7 + short_21_8 + short_21_9 + short_21_10 + short_21_11 + short_21_12 + short_21_13 + short_21_14 + short_21_15 + short_21_16 + short_21_17 + short_21_18 + short_21_19 + short_21_20 + short_21_21 + short_21_22 + short_21_23 + short_21_24 + short_21_25 + short_21_26]
  ask node 22 [set short_Em short_22_0 + short_22_1 + short_22_2 + short_22_3 + short_22_4 + short_22_5 + short_22_6 + short_22_7 + short_22_8 + short_22_9 + short_22_10 + short_22_11 + short_22_12 + short_22_13 + short_22_14 + short_22_15 + short_22_16 + short_22_17 + short_22_18 + short_22_19 + short_22_20 + short_22_21 + short_22_22 + short_22_23 + short_22_24 + short_22_25 + short_22_26]
  ask node 23 [set short_Im short_23_0 + short_23_1 + short_23_2 + short_23_3 + short_23_4 + short_23_5 + short_23_6 + short_23_7 + short_23_8 + short_23_9 + short_23_10 + short_23_11 + short_23_12 + short_23_13 + short_23_14 + short_23_15 + short_23_16 + short_23_17 + short_23_18 + short_23_19 + short_23_20 + short_23_21 + short_23_22 + short_23_23 + short_23_24 + short_23_25 + short_23_26]
  ask node 24 [set short_Am short_24_0 + short_24_1 + short_24_2 + short_24_3 + short_24_4 + short_24_5 + short_24_6 + short_24_7 + short_24_8 + short_24_9 + short_24_10 + short_24_11 + short_24_12 + short_24_13 + short_24_14 + short_24_15 + short_24_16 + short_24_17 + short_24_18 + short_24_19 + short_24_20 + short_24_21 + short_24_22 + short_24_23 + short_24_24 + short_24_25 + short_24_26]
  ask node 25 [set short_t short_25_0 + short_25_1 + short_25_2 + short_25_3 + short_25_4 + short_25_5 + short_25_6 + short_25_7 + short_25_8 + short_25_9 + short_25_10 + short_25_11 + short_25_12 + short_25_13 + short_25_14 + short_25_15 + short_25_16 + short_25_17 + short_25_18 + short_25_19 + short_25_20 + short_25_21 + short_25_22 + short_25_23 + short_25_24 + short_25_25 + short_25_26]
  ask node 26 [set short_Xm short_26_0 + short_26_1 + short_26_2 + short_26_3 + short_26_4 + short_26_5 + short_26_6 + short_26_7 + short_26_8 + short_26_9 + short_26_10 + short_26_11 + short_26_12 + short_26_13 + short_26_14 + short_26_15 + short_26_16 + short_26_17 + short_26_18 + short_26_19 + short_26_20 + short_26_21 + short_26_22 + short_26_23 + short_26_24 + short_26_25 + short_26_26]

;  ask node 0 [show short_i]
;  ask node 1 [show short_TR]
;  ask node 2 [show short_R]
;  ask node 3 [show short_F]
;  ask node 4 [show short_T]
;  ask node 5 [show short_n]
;  ask node 6 [show short_S]
;  ask node 7 [show short_Cp]
;  ask node 8 [show short_pHg]
;  ask node 9 [show short_Xg]
;  ask node 10 [show short_Cc]
;  ask node 11 [show short_foc]
;  ask node 12 [show short_pHw]
;  ask node 13 [show short_Tw]
;  ask node 14 [show short_pw]
;  ask node 15 [show short_Ew]
;  ask node 16 [show short_Iw]
;  ask node 17 [show short_Aw]
;  ask node 18 [show short_DOC]
;  ask node 19 [show short_pHm]
;  ask node 20 [show short_Tm]
;  ask node 21 [show short_pm]
;  ask node 22 [show short_Em]
;  ask node 23 [show short_Im]
;  ask node 24 [show short_Am]
;  ask node 25 [show short_t]
;  ask node 26 [show short_Xm]

  ask nodes [set short short_i + short_TR + short_R + short_F + short_T + short_n + short_S + short_Cp + short_pHg + short_Xg + short_Cc + short_foc + short_pHw + short_Tw + short_pw + short_Ew + short_Iw + short_Aw + short_DOC + short_pHm + short_Tm + short_pm + short_Em + short_Im + short_Am + short_t + short_Xm]
 ; ask nodes [show short]
  set pathlength sum[short] of nodes
  print "Summation of the shortest pathlengths of all the nodes in the network"
  show pathlength

;  ask nodes [set path path0 + path1 + path2 + path3 + path4 + path5 + path6 + path7 + path8 + path9 + path10 + path11 + path12 + path13 + path14 + path15 + path16 + path17 + path18 + path19 + path20 + path21 + path22 + path23 + path24 + path25 + path26]
;  set possiblepaths sum[path] of nodes
;  show possiblepaths

  print "Characteristic pathlength of the network"
  set CharPL (pathlength)/(N * (N - 1))
  show CharPL

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
  ask node 26 [ set cluster25 [nw:clustering-coefficient] of node 26 ]

print "Clustering coefficient of all factors in the NoF"

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
  ask node 26 [ show cluster26 ]

  set Mean_cluster mean[nw:clustering-coefficient] of nodes
  print "Clustering coefficient of the network"
  show Mean_cluster


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

to go-target-id
  ;; if the below condition is true then we have a fully disconnected network and we need to stop
  if (count links = 0) [
    display
    user-message "Network is fully disconnected. No more edges can be removed."
    stop
  ]


  remove-edge-attack-id
  find-all-components-new
  color-giant-component
  ask links [ set color [color] of end1 ]  ;; recolor all edges
  layout-1
  tick
end

to go-target-od
  ;; if the below condition is true then we have a fully disconnected network and we need to stop
  if (count links = 0) [
    display
    user-message "Network is fully disconnected. No more edges can be removed."
    stop
  ]


  remove-edge-attack-od
  find-all-components-new
  color-giant-component
  ask links [ set color [color] of end1 ]  ;; recolor all edges
  layout-1
  tick
end

to go-target-cc
  ;; if the below condition is true then we have a fully disconnected network and we need to stop
  if (count links = 0) [
    display
    user-message "Network is fully disconnected. No more edges can be removed."
    stop
  ]


  remove-edge-attack-cc
  find-all-components-new
  color-giant-component
  ask links [ set color [color] of end1 ]  ;; recolor all edges
  layout-1
  tick
end

to go-target-bc
  ;; if the below condition is true then we have a fully disconnected network and we need to stop
  if (count links = 0) [
    display
    user-message "Network is fully disconnected. No more edges can be removed."
    stop
  ]


  remove-edge-attack-bc
  find-all-components-new
  color-giant-component
  ask links [ set color [color] of end1 ]  ;; recolor all edges
  layout-1
  tick
end

to go-target-ec
  ;; if the below condition is true then we have a fully disconnected network and we need to stop
  if (count links = 0) [
    display
    user-message "Network is fully disconnected. No more edges can be removed."
    stop
  ]


  remove-edge-attack-ec
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

;; pick a node and remove its link based on in-degree centrality

to remove-edge-attack-id

    ask nodes [ set indeg count my-in-links]
    ask one-of nodes with [indeg = max [count my-in-links] of nodes] [
    ifelse (count my-in-links = 0) [
    remove-edge-attack-id
    ]

    [set color red
    ask my-links [die]
            ]
    ]

end

;; pick a node and remove its link based on out-degree centrality

to remove-edge-attack-od

    ask nodes [ set outdeg count my-out-links]
    ask one-of nodes with [outdeg = max [count my-out-links] of nodes] [
    ifelse (count my-out-links = 0) [
    remove-edge-attack-od
    ]

    [set color red
    ask my-links [die]
            ]
    ]

end

;; pick a node and remove its link based on closeness centrality

to remove-edge-attack-cc

 ask nodes [ set closeness nw:closeness-centrality ]
    ask one-of nodes with [closeness = max [nw:closeness-centrality] of nodes] [
    ifelse (count my-links = 0) [
    remove-edge-attack-cc
    ]

     [set color red
    ask my-links [die]
            ]
    ]

end

;; pick a node and remove its link based on betweenness centrality

to remove-edge-attack-bc

 ask nodes [ set betweenness nw:betweenness-centrality ]
    ask one-of nodes with [betweenness = max [nw:betweenness-centrality] of nodes] [
    ifelse (count my-links = 0) [
    remove-edge-attack-bc
    ]

     [set color red
    ask my-links [die]
            ]
    ]

end

;; pick a node and remove its link based on eigenvector centrality

to remove-edge-attack-ec

 ask nodes [ set eigenvector nw:eigenvector-centrality ]
    ask one-of nodes with [eigenvector = max [nw:eigenvector-centrality] of nodes] [
    ifelse (count my-links = 0) [
    remove-edge-attack-ec
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
  layout-spring nodes links 0.2 8 0.2

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
