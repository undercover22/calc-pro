# calc-pro









:"ABCDEFGHIJKLMNOPQRSTUVWXYZ→Str0
:Repeat 30>length(Str1
:ClrHome
:Disp "ENTER A WORD: (29 CHARS)
:Input "",Str1
:End
:"GUESS A LETTER:→Str2
:For(I,1,length(Str1
:sub(Str1,I,1
:If inString(Str0,Ans:"-
:Str2+Ans→Str2
:End
:sub(Ans,2,length(Ans)-1→Str2
:8→T
:ClrHome
:While Str1≠Str2 and T
:Output(1,1,Str2
:.1{69,67,58,49,47,48,38,38
:Output(iPart(Ans(T)),10fPart(Ans(T)),sub("^^I--IO ",T,1
:Repeat 30<Ans and Ans<94
:getKey
:End
:If Ans=45:Goto Q
:Ans-20-5int(.1Ans)-2(Ans>45→K
:sub(Str0,Ans,1→Str3
:Output(7+(K>14),K+1-13(K>14),Ans
:inString(Str1,Ans→I
:T-not(Ans→T
:While I
:sub(sub(" "+Str2,1,I)+Str3+sub(Str2+" ",I+1,length(Str2)-I+1),2,length(Str2→Str2
:inString(Str1,Str3,I+1→I
:End
:End
:Lbl Q
:Pause "YOU "+sub("LOSE!WIN! ",1+5(Str1=Str2),5
:ClrHome






