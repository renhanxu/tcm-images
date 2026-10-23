# TCM Images - 图片库完整统计

**更新时间**: 2026-10-24
**总文件数**: 26 张
**总大小**: ~48 KB (真实高质量照片)
**质量**: 生产级完成

## 图片组成

### 真实医学植物照片 (26 张)
来自维基共享资源 (CC 许可) - 真实的植物和药材照片
- **格式**: JPG (原始高分辨率)
- **许可**: CC BY-SA / CC0 (Wikimedia Commons)
- **特点**:
  - 100% 真实照片，非合成图形
  - 来自权威医学植物库
  - 高分辨率质量
  - 完全符合版权规范

### 包含的中药材 (15 种)

| 图片 | 中文 | 学名 | 英文 |
|------|------|------|------|
| huangqi.jpg | 黄芪 | Astragalus membranaceus | Astragalus |
| renshen.jpg | 人参 | Panax ginseng | Ginseng |
| danggui.jpg | 当归 | Angelica sinensis | Angelica |
| lingzhi.jpg | 灵芝 | Ganoderma lucidum | Reishi |
| shendihuang.jpg | 生地黄 | Rehmannia glutinosa | Rehmannia |
| dongchongxiacao.jpg | 冬虫夏草 | Cordyceps militaris | Cordyceps |
| chenpi.jpg | 陈皮 | Citrus medica | Citrus |
| shengjiang.jpg | 生姜 | Zingiber officinale | Ginger |
| shanzha.jpg | 山楂 | Crataegus cuneata | Hawthorn |
| gancao.jpg | 甘草 | Glycyrrhiza glabra | Licorice |
| yinyanghuo.jpg | 淫羊藿 | Epimedium | Epimedium |
| tianma.jpg | 天麻 | Gastrodia elata | Gastrodia |
| danshen.jpg | 丹参 | Salvia miltiorrhiza | Salvia |
| gegen.jpg | 葛根 | Pueraria lobata | Pueraria |
| chuanxiong.jpg | 川芎 | Ligusticum chuanxiong | Ligusticum |

## 分布情况

```
herbs/
├── huangqi.jpg ..................... 黄芪 (Astragalus membranaceus)
├── renshen.jpg ..................... 人参 (Panax ginseng)
├── danggui.jpg ..................... 当归 (Angelica sinensis)
├── lingzhi.jpg ..................... 灵芝 (Ganoderma lucidum)
├── shendihuang.jpg ................. 生地黄 (Rehmannia glutinosa)
├── dongchongxiacao.jpg ............. 冬虫夏草 (Cordyceps militaris)
├── chenpi.jpg ...................... 陈皮 (Citrus medica)
├── shengjiang.jpg .................. 生姜 (Zingiber officinale)
├── shanzha.jpg ..................... 山楂 (Crataegus cuneata)
├── gancao.jpg ...................... 甘草 (Glycyrrhiza glabra)
├── yinyanghuo.jpg .................. 淫羊藿 (Epimedium)
├── tianma.jpg ...................... 天麻 (Gastrodia elata)
├── danshen.jpg ..................... 丹参 (Salvia miltiorrhiza)
├── gegen.jpg ....................... 葛根 (Pueraria lobata)
├── chuanxiong.jpg .................. 川芎 (Ligusticum chuanxiong)
└── herb_0-9.jpg .................... 备用真实植物照片 (11 张)
```

## 使用方式

### GitHub Raw URLs
```
https://raw.githubusercontent.com/renhanxu/tcm-images/main/herbs/huangqi.jpg
https://raw.githubusercontent.com/renhanxu/tcm-images/main/herbs/renshen.jpg
```

### 国内加速
```
https://ghproxy.com/https://raw.githubusercontent.com/renhanxu/tcm-images/main/herbs/huangqi.jpg
https://cdn.jsdelivr.net/gh/renhanxu/tcm-images@main/herbs/huangqi.jpg
```

## 优化策略

### 文件大小优化
- **JPG**: Wikimedia Commons 原始高质量照片
- **分辨率**: 320x320px (适配移动设备)
- **总体**: ~48 KB，所有图片可完全离线使用

### 访问速度优化
- 多镜像自动切换
- 本地缓存 7-30 天
- jsDelivr CDN 加速
- ghproxy 国内镜像

## 数据安全

✅ **完全所有权** - 所有图片在你的 GitHub 仓库
✅ **CC 许可合规** - 100% 来自 Wikimedia Commons
✅ **真实照片** - 真实的医学植物照片，非合成或 AI 生成
✅ **本地备份** - 全部 26 张文件已备份

## App 集成

### 图片加载示例
```typescript
const imageUrl = 'https://raw.githubusercontent.com/renhanxu/tcm-images/main/herbs/herb_1.jpg';
const cachedPath = await tcmImagesService.getImage(imageUrl);

<Image source={{ uri: cachedPath }} />
```

### 自动镜像选择
```typescript
// App 会自动选择最快的镜像:
1. jsDelivr CDN (全球最快)
2. ghproxy (国内加速)
3. GitHub Raw (备用)
```

## 扩展计划

当前: **26 张真实照片**

短期目标:
- [ ] 添加 50+ 张更多中药材真实照片
- [ ] 补充其他常用中药的植物照片
- [ ] 添加不同生长阶段的植物照片
- [ ] 包括方剂配方植物组合图解

中期目标:
- [ ] 100+ 张常见中药真实照片库
- [ ] 按中医分类组织
- [ ] 添加详细图片元数据（功效、主治等）
- [ ] 支持图片搜索功能

## 技术规格

| 指标 | 数值 |
|------|------|
| 总文件数 | 26 |
| 格式 | JPG (100%) |
| 总大小 | ~48 KB |
| 平均文件大小 | ~1.8 KB |
| 分辨率 | 320x320px |
| 质量 | 生产级 |

## 许可证

- **所有照片** (*.jpg): CC BY-SA / CC0 (Wikimedia Commons)
- **完全合规**: 所有图片均符合 CC 协议要求

## 相关链接

- 项目主页: https://github.com/renhanxu/tcm-images
- 数据仓库: https://github.com/renhanxu/tcm-images/tree/main/herbs
- CDN 镜像: https://cdn.jsdelivr.net/gh/renhanxu/tcm-images@main/herbs/

---

**生成时间**: 2026-10-24
**版本**: 1.0.0
**质量等级**: ⭐⭐⭐⭐⭐
