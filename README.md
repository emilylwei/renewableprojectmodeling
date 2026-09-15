#simplecalculations
capacity_mw = 100
capacity_factor = 0.25
ppa_price_per_mwh = 50
capex_per_kw = 1200
annual_opex = 2_000_000

hours_per_year = 8760

annual_generation_mwh = capacity_mw * hours_per_year * capacity_factor
annual_revenue = annual_generation_mwh * ppa_price_per_mwh

capacity_kw = capacity_mw * 1000
total_capex = capacity_kw * capex_per_kw

annual_operating_cash_flow = annual_revenue - annual_opex

print("Annual generation:", annual_generation_mwh, "MWh")
print("Annual revenue: $", annual_revenue)
print("Total CapEx: $", total_capex)
print("Annual operating cash flow: $", annual_operating_cash_flow)
