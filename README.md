# n8n Agent IA Coderhouse

Workflow desarrollado en n8n como parte de una práctica de automatización
con inteligencia artificial.

## Descripción

El workflow implementa un AI Agent configurado como Tools Agent.

El agente utiliza:

- OpenAI Chat Model
- Google Sheets como herramienta
- Máximo de 8 iteraciones
- System Message operativo
- Ejecución manual mediante Manual Trigger

## Arquitectura

Manual Trigger
→ AI Agent
→ OpenAI Chat Model

AI Agent
→ Google Sheets Tool

## Funcionamiento

El agente analiza la solicitud recibida y determina si necesita consultar
información almacenada en Google Sheets.

La herramienta Google Sheets está configurada con la operación Get Row(s),
permitiendo al agente recuperar información de la hoja cuando la solicitud
lo requiere.

## Archivo

El workflow completo se encuentra en:

`n8n-tools-agent-google-sheets.json`
