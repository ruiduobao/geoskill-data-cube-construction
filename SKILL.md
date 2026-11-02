---
name: geoskill-data-cube-construction
description: '把多时相多波段影像组织为带坐标的 xarray/NetCDF 数据立方体，支持离线合成模式'
---

# 遥感数据立方体构建 | Remote Sensing Data Cube Construction

(Fill in 2-3 paragraphs of Chinese introduction here: features, application scenarios, core algorithms.)

## Dependencies / 依赖

```bash
pip install 'numpy' 'rasterio' 'xarray' 'netcdf4'
```

## Usage / 使用方法

### Basic Usage

```bash
python geoskill-data-cube-construction.py --bbox 116.0 39.0 117.0 40.0 [other parameters]
```

### Example 1 (synthetic data, offline)

```bash
python geoskill-data-cube-construction.py --bbox 116.0 39.0 117.0 40.0 --synthetic --output-dir ./out
```

### Examples 2-5

(Add at least 4 real usage examples.)

## Output / 输出

| File | Format | Description |
|---|---|---|
| `result.tif` | GeoTIFF | Primary output |
| `output-manifest.json` | JSON | Run manifest |

## Data Source / 数据源 / Source

(Describe the data source: free satellite data / local input / synthetic.)

## Privacy / 隐私声明 / Privacy

- Runs offline by default; `--synthetic` mode requires no network at all.
- All processing is done locally; no user data is uploaded.

## License / License

MIT

---

> 中文完整版：需要时再读 [references/SKILL.zh-CN.md](references/SKILL.zh-CN.md)，不要默认全量加载。
