## 📌 Descripción del proyecto

Análisis integral de un e-commerce simulado con datos reales de operación: ventas, compras, stock, devoluciones, comisiones, facturación e IVA. El proyecto abarca desde la exploración y limpieza de datos hasta la construcción de dashboards ejecutivos orientados a la toma de decisiones comerciales y financieras.

Desarrollado como proyecto de portfolio para demostrar competencias en **análisis de datos**, **business intelligence** y **análisis financiero/contable**.

---

## 📊 Dashboards

### 1. Dashboard Comercial
Visión general del negocio: ingresos, canales de venta, categorías de productos, devoluciones y mix de ventas.

**Métricas clave:**
- Ingresos brutos: **$65.2B** | Ingresos netos: **$58.5B**
- Ticket promedio: **$652K** | 15.2 unidades por venta
- Canal online: **57%** | Tienda física: **43%**
- Devoluciones: **$371M** en 2.000 casos

### 2. Dashboard Financiero / Contable
Análisis de cashflow, posición de IVA, cuotas cobradas y por cobrar, y estado de resultados estimado.

**Métricas clave:**
- Cuotas cobradas 2025: **$57.9B** (88.8% del total)
- Cuotas por cobrar 2026: **$7.3B** (concentradas en Q1)
- IVA a pagar neto: **$3.6B** | Posición: siempre a pagar
- Resultado neto estimado: **$47.8B** (margen ~73%)

---

## 🗂️ Estructura del dataset

| Hoja | Descripción | Registros |
|------|-------------|-----------|
| `productos` | Catálogo con precios, costos, dimensiones y popularidad | 197 |
| `ventas` | Transacciones con canal, cantidad, cuotas e ingreso | 100.000 |
| `cuotas` | Detalle de cobros por cuota (2025–2026) | 368.958 |
| `compras` | Órdenes a proveedores con IVA y tipo de factura | ~8.000 |
| `stock` | Entradas, salidas y alertas de reposición | 4.988 alertas |
| `facturas_emitidas` | Facturas A y B con IVA discriminado | 100.000 |
| `devoluciones` | Motivos y montos de devolución | 2.000 |
| `comisiones` | Comisiones por canal (online 15% / tienda 5%) | 100.000 |
| `libro_iva` | Débito, crédito y posición fiscal mensual | 12 meses |

---

## 🛠️ Tecnologías utilizadas

| Herramienta | Uso |
|-------------|-----|
| **Python** (pandas, numpy) | ETL, limpieza y análisis exploratorio |
| **Excel** | Dataset fuente con múltiples hojas relacionadas |
| **Chart.js** | Visualizaciones interactivas en HTML |
| **HTML / CSS** | Dashboards autocontenidos descargables |

---

## 💡 Principales insights

- **Estacionalidad plana**: los ingresos son estables mes a mes (~$5.4B–$5.7B), sin picos estacionales marcados.
- **Canal online dominante** en volumen (57%) pero con mayor costo de comisión (15% vs 5% tienda).
- **Cuotas 2026**: el 11.2% del ingreso 2025 aún no fue cobrado; el 34% de esa deuda vence en enero 2026.
- **IVA siempre a pagar**: el crédito fiscal (compras) representa solo el ~13% del débito fiscal (ventas).
- **Devoluciones distribuidas**: ningún motivo supera el 22% del total — problema sistémico, no puntual.
- **Stock crítico**: 4.988 productos con alerta de reposición activa.

---

## 📁 Archivos del proyecto

```
├── portfolio_ecommerce.xlsx       # Dataset fuente (9 hojas)
├── dashboard_ecommerce_2025.html  # Dashboard comercial (abrir en navegador)
├── dashboard_financiero_2025.html # Dashboard financiero (abrir en navegador)
└── README.md                      # Este archivo
```

---

## 👤 Autor

**Gonzalo Dalmasso Müller**
Business & Data Analyst | SQL · Python · Power BI · Tableau · Looker Studio

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Gonzalo%20Dalmasso-0077B5?style=flat&logo=linkedin)](https://linkedin.com/in/gonzalo-dalmasso-486094206)
📧 gonzalodalmasso7@hotmail.com

---
---

# English Version

# 🛒 E-Commerce Analytics Project — Full Business Analysis

## 📌 Project Overview

End-to-end analysis of a simulated e-commerce operation with realistic data: sales, purchases, inventory, returns, commissions, invoicing, and VAT. The project covers everything from data exploration and cleaning to the development of executive dashboards for both commercial and financial decision-making.

Built as a portfolio project to showcase skills in **data analysis**, **business intelligence**, and **financial/accounting analysis**.

---

## 📊 Dashboards

### 1. Commercial Dashboard
Business overview: revenue, sales channels, product categories, returns, and sales mix.

**Key metrics:**
- Gross revenue: **$65.2B** | Net revenue: **$58.5B**
- Average ticket: **$652K** | 15.2 units per transaction
- Online channel: **57%** | Physical store: **43%**
- Returns: **$371M** across 2,000 cases

### 2. Financial / Accounting Dashboard
Cash flow analysis, VAT position, collected and outstanding installments, and estimated P&L.

**Key metrics:**
- Installments collected in 2025: **$57.9B** (88.8% of total)
- Outstanding installments for 2026: **$7.3B** (concentrated in Q1)
- Net VAT payable: **$3.6B** | Always in payable position
- Estimated net income: **$47.8B** (~73% margin)

---

## 🗂️ Dataset Structure

| Sheet | Description | Records |
|-------|-------------|---------|
| `productos` | Product catalog with prices, costs, dimensions, and popularity | 197 |
| `ventas` | Transactions with channel, quantity, installments, and revenue | 100,000 |
| `cuotas` | Installment payment schedule (2025–2026) | 368,958 |
| `compras` | Supplier orders with VAT and invoice type | ~8,000 |
| `stock` | Stock entries, exits, and replenishment alerts | 4,988 alerts |
| `facturas_emitidas` | A and B invoices with itemized VAT | 100,000 |
| `devoluciones` | Return reasons and amounts | 2,000 |
| `comisiones` | Channel commissions (online 15% / store 5%) | 100,000 |
| `libro_iva` | Monthly VAT debit, credit, and tax position | 12 months |

---

## 🛠️ Tech Stack

| Tool | Usage |
|------|-------|
| **Python** (pandas, numpy) | ETL, cleaning, and exploratory analysis |
| **Excel** | Source dataset with multiple related sheets |
| **Chart.js** | Interactive HTML visualizations |
| **HTML / CSS** | Self-contained downloadable dashboards |

---

## 💡 Key Insights

- **Flat seasonality**: monthly revenue is stable (~$5.4B–$5.7B) with no marked seasonal peaks.
- **Online channel leads** in volume (57%) but carries higher commission cost (15% vs 5% in-store).
- **2026 receivables**: 11.2% of 2025 revenue is still uncollected; 34% of that debt matures in January 2026.
- **VAT always payable**: tax credit (purchases) represents only ~13% of tax debit (sales).
- **Distributed returns**: no single reason exceeds 22% of total — a systemic issue, not an isolated one.
- **Critical stock**: 4,988 products currently flagged for replenishment.

---

## 📁 Project Files

```
├── portfolio_ecommerce.xlsx       # Source dataset (9 sheets)
├── dashboard_ecommerce_2025.html  # Commercial dashboard (open in browser)
├── dashboard_financiero_2025.html # Financial dashboard (open in browser)
└── README.md                      # This file
```

---

## 👤 Author

**Gonzalo Dalmasso Müller**
Business & Data Analyst | SQL · Python · Power BI · Tableau · Looker Studio

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Gonzalo%20Dalmasso-0077B5?style=flat&logo=linkedin)](https://linkedin.com/in/gonzalo-dalmasso-486094206)
📧 gonzalodalmasso7@hotmail.com
