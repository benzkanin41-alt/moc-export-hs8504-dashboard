# Thailand Export Monitor: หม้อแปลงไฟฟ้า HS 8504

Static dashboard สำหรับติดตามยอดส่งออกไทยของหม้อแปลงไฟฟ้าและสินค้าที่อยู่ใน HS Code 8504

## Online Dashboard

เมื่อเปิด GitHub Pages แล้ว dashboard จะอยู่ที่:

```text
https://benzkanin41-alt.github.io/moc-export-hs8504-dashboard/
```

## Source

- Source: Thailand Trade Report, Ministry of Commerce
- Report page: https://tradereport.moc.go.th/th/stat/reporthscodeexport01
- Endpoint: `https://tradereport.moc.go.th/stat/reporthscodeexport01/result`
- HS Code: `8504`
- HS version: `2022`
- Product name from MOC: `8504 : หม้อแปลงไฟฟ้า เครื่องเปลี่ยนไฟฟ้าชนิดอยู่คงที่ (สแตติกคอนเวอร์เตอร์) (เช่น เครื่องกลับกระแสไฟฟ้า) และตัวเหนี่ยวนา`
- Coverage: `2021-01` ถึง `2026-07`
- Latest source month: `ก.ค. 2569`

## Validation

- Months fetched: `67`
- Country-month rows: `7,287`
- Max value reconciliation diff: `0.0`
- Max quantity reconciliation diff: `0.0`
- Unmapped country IDs: none

## Quantity Caveat

MOC คืนค่า `QuantityMonth = 0` ทุกเดือนสำหรับ HS 8504 ในชุดข้อมูลนี้ จึงแสดง field ปริมาณใน dashboard เป็น `ไม่รายงาน` ใน KPI หลัก เพื่อไม่ให้ตีความผิดว่า volume จริงเป็นศูนย์

## Included Files

- `index.html` dashboard shell
- `styles.css` responsive dashboard styling
- `app.js` interactive charts, filters, table sorting, CSV export
- `data.js` embedded dashboard dataset
- `data/dataset.json` full source-backed dataset
- `data/monthly_country_hs8504.csv`
- `data/monthly_continent_hs8504.csv`
- `data/monthly_total_hs8504.csv`
- `data/validation_reconciliation.csv`
