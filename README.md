# -primeros-ejercicios-de-Python-2026
“primeros ejercicios de Python, 2026
maquinas = [
    {"nombre": "Prensa", "temperatura": 110, "ciclos": 1800, "vibracion": 4},
    {"nombre": "Robot", "temperatura": 95, "ciclos": 400, "vibracion": 7},
    {"nombre": "Soldadora", "temperatura": 70, "ciclos": 300, "vibracion": 2},
    {"nombre": "Cinta", "temperatura": 45, "ciclos": 1200, "vibracion": 1},
    {"nombre": "Torno", "temperatura": 85, "ciclos": 2000, "vibracion": 6},
    {"nombre": "Taladro", "temperatura": 105, "ciclos": 500, "vibracion": 3},
    {"nombre": "Transportador", "temperatura": 60, "ciclos": 1000, "vibracion": 5},
    {"nombre": "Pulidora", "temperatura": 90, "ciclos": 1600, "vibracion": 2},
    {"nombre": "Empacadora", "temperatura": 120, "ciclos": 1800, "vibracion": 6},
    {"nombre": "Mezcladora", "temperatura": 80, "ciclos": 1400, "vibracion": 4}
]


for maquina in maquinas:
    alertas_maquina = []
   
    if maquina['temperatura']> 100:
     alertas_maquina.append("TEMPERATURA ALTA")
   
    if maquina['temperatura'] < 50 :
     alertas_maquina.append("temperatura baja ")
   
    if maquina['ciclos'] > 1500:
      alertas_maquina.append ("MANTENIMIENTO PRONTO")
    
    if maquina['vibracion'] > 5:
      alertas_maquina.append ("vibracion alta")

    print(f"{maquina['nombre']} :  {",".join(alertas_maquina)} alertas: {len(alertas_maquina)}")
