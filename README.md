# osu-stats-signature

## 简介

osu-stats-signature 可以生成实时更新的 osu! 个人资料卡片/签名档。生成的卡片为 SVG，可用于个人主页。

## 本Fork 简介

本人打算在一个校园博客（迫真）上插入'osu-stats-signature'，奈何博客禁用了'<iframe>'、'<embed>'、'<script>'、带有传参的url（这直接导致我难以使用原项目的api）以及base64嵌入，故Fork了一份并修改了不传入'username'时的默认参数（这样不用传参也可以使用api了）。

## 使用

该项目部署在 Vercel 上，前往 [osu-stats-signature.vercel.app](https://osu-stats-signature.vercel.app) 生成卡片。

将得到的卡片 SVG 地址作为图片插入到个人主页中即可。

## 功能 & TODO

- [x] 获取 osu! 账号信息并生成卡片
- [x] 获取并显示头像和用户背景图片
- [x] 支持背景图片高斯模糊
- [x] 过渡动画
- [x] 显示 Supporter Tag
- [x] 英文版卡片
- [x] Mini 卡片
- [x] 缓存机制
- [ ] 生成个人 bp (最佳成绩) 卡片
- [ ] 生成单个成绩详情卡片

# 预览

## Full

<a href="https://osu.ppy.sh/users/7562902/"><img src="https://osu-sig.vercel.app/card?user=mrekk&mode=std&lang=en&animation=true" width="550" /></a>

<a href="https://osu.ppy.sh/users/21226378/"><img src="https://osu-sig.vercel.app/card?user=solstice23&mode=std&animation=true" width="550" /></a>

### With osu!skills chart

<a href="https://osu.ppy.sh/users/7562902/"><img src="https://osu-sig.vercel.app/card?user=mrekk&mode=std&lang=en&animation=true&skills=true&hue=255" width="550" /></a>

## Mini

<a href="https://osu.ppy.sh/users/21226378/"><img src="https://osu-sig.vercel.app/card?user=solstice23&mode=std&blur=6&animation=true&mini=true" width="400" /></a>
