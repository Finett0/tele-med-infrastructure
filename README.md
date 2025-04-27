# TeleMed-infrastructure

#  Aplicativo Médico para Consultas Online

Aplicativo médico que permite a realização de consultas entre médicos e pacientes por meio de videochamada.  
Ao final da consulta, o médico pode emitir atestados ou receitas digitais, que são armazenados na nuvem e disponibilizados ao paciente via link enviado por SMS.

---

## Funcionalidades

- Videochamada entre paciente e médico via web
- Geração de documentos (atestado/receita) após a consulta
- Armazenamento seguro dos documentos na nuvem
- Envio de link via SMS para o paciente acessar seus documentos

---

## Componentes Técnicos (AWS)

- **AWS S3 + CloudFront** — Hospedagem do frontend (app web)
- **AWS API Gateway + AWS Lambda** — Backend com API REST
- **Amazon Chime SDK** — Serviço de videochamada
- **AWS Lambda** — Geração de atestado/receita
- **AWS S3** — Armazenamento de arquivos
- **AWS SNS** — Envio de SMS
- **AWS RDS** — Banco de dados

---

## Como funciona?

1. Paciente acessa o app web hospedado em S3/CloudFront.
2. Realiza a videochamada com o médico (Chime SDK).
3. Após a consulta, o médico gera documentos digitais (Lambda).
4. Documentos são armazenados no S3 de forma segura.
5. Um link para o documento é enviado ao paciente via SMS (SNS).

---

## 📄 Licença

Este projeto está licenciado sob a licença MIT.  
Sinta-se livre para usar, modificar e melhorar!

---




https://excalidraw.com/#json=cJte9xKtWeeiXWWheT9EX,ycN-mWf24ozhDJjowO0cDw
