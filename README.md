# AbisSol – Sistema de Telemetria para Barco Solar

Sistema de monitoramento em tempo real para embarcação solar, desenvolvido para competições DSB.

## Tecnologias
- C++ (ESP32/Arduino)
- Python (análise e visualização)
- Sensores: INA226 (tensão/corrente), DS18B20 (temperatura)
- Protocolos: I2C, OneWire
- Filtros digitais de média móvel
- Máquina de estados para alertas (NORMAL/ALERTA/CRÍTICO)

## Funcionalidades
- Leitura de tensão, corrente, potência, temperatura
- Cálculo de SoC (State of Charge) e autonomia estimada
- Detecção de sobrecarga, superaquecimento, baixa bateria
- Logging em JSON para análise posterior
- Transmissão de dados para cockpit

## Exemplo de saída (JSON)
```json
{
  "METADADOS": {
    "projeto": "DSB Telemetria Pro",
    "equipe": "Barco Solar DSB",
    "versao_firmware": 2.9,
    "timestamp_gravacao_utc": "2026-05-17T19:30:00Z"
  }
}
