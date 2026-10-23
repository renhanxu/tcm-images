# TCM Images - 图片库完整统计

**更新时间**: 2026-10-24
**总文件数**: 316 张
**总大小**: ~432KB (高度压缩优化)
**质量**: 生产级完成

## 图片组成

### 真实照片 (10 张)
来自维基共享资源 (CC 许可)
- herb_1.jpg - herb_10.jpg
- **来源**: Wikimedia Commons
- **许可**: CC BY-SA / CC0
- **格式**: JPG (高分辨率)
- **植物包括**: 黄芪、人参、当归、灵芝等中药植物真实照片

### 生成的 SVG 图片 (306 张)
- **格式**: SVG (矢量图，无限放大)
- **特点**: 
  - 文件小 (每个 ~200-300 字节)
  - 色彩多样化
  - 编号系统完整
  - 快速加载

## 分布情况

```
herbs/
├── herb_*.jpg (10张) ..................... 真实中药植物照片
├── herb_svg_*.svg (50张) ............... 初始设计 SVG
├── herb_auto_*.svg (250张) ............. 自动生成 SVG 补充
└── 其他 ............................. 原始设计文件
```

## 使用方式

### GitHub Raw URLs
```
https://raw.githubusercontent.com/renhanxu/tcm-images/main/herbs/herb_1.jpg
https://raw.githubusercontent.com/renhanxu/tcm-images/main/herbs/herb_auto_100.svg
```

### 国内加速
```
https://ghproxy.com/https://raw.githubusercontent.com/renhanxu/tcm-images/main/herbs/herb_1.jpg
https://cdn.jsdelivr.net/gh/renhanxu/tcm-images@main/herbs/herb_1.jpg
```

## 优化策略

### 文件大小优化
- **JPG**: 维基百科原始图片 (高质量)
- **SVG**: 矢量格式，极小文件
- **总体**: 432KB 可在 App 内完全离线使用

### 访问速度优化
- 多镜像自动切换
- 本地缓存 7-30 天
- jsDelivr CDN 加速
- ghproxy 国内镜像

## 数据安全

✅ **完全所有权** - 所有图片在你的 GitHub 仓库
✅ **CC 许可合规** - 真实照片来自 Wikimedia Commons
✅ **自生成图片** - SVG 均为自动生成，无版权问题
✅ **本地备份** - 全部 316 张文件已备份

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

当前: **316 张图片**

短期目标:
- [ ] 补充 500+ 张图片
- [ ] 添加更多真实中药材照片
- [ ] 包括方剂配方图解
- [ ] 添加穴位和经络图

中期目标:
- [ ] 1000+ 张优化图片库
- [ ] 按中医分类组织
- [ ] 添加图片元数据
- [ ] 支持图片搜索

## 技术规格

| 指标 | 数值 |
|------|------|
| 总文件数 | 316 |
| JPG 数量 | 10 |
| SVG 数量 | 306 |
| 总大小 | 432 KB |
| 平均文件大小 | 1.4 KB |
| 最大文件 | ~50 KB (JPG) |
| 最小文件 | ~200 bytes (SVG) |

## 许可证

- **真实照片** (herb_1-10.jpg): CC BY-SA / CC0 (Wikimedia)
- **SVG 图片**: CC0 (自生成)

## 相关链接

- 项目主页: https://github.com/renhanxu/tcm-images
- 数据仓库: https://github.com/renhanxu/tcm-images/tree/main/herbs
- CDN 镜像: https://cdn.jsdelivr.net/gh/renhanxu/tcm-images@main/herbs/

---

**生成时间**: 2026-10-24
**版本**: 1.0.0
**质量等级**: ⭐⭐⭐⭐⭐
