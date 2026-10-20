# Pablo Alberto Duque Marín

**Ingeniero de IA** en Caldas, Colombia (remoto, UTC−5). Llevo IA generativa a producción sobre AWS:
pipelines de documentos, RAG y agentes con Amazon Bedrock, con la infraestructura en Terraform y
pruebas automatizadas. Mido con estadística si funcionan, con el protocolo fijado antes de ver los
datos, y publico también los resultados negativos.

Disponible: freelance ahora · tiempo completo desde enero de 2027 · remoto.

[pabloduque.dev](https://pabloduque.dev) · [LinkedIn](https://www.linkedin.com/in/pablo-alberto-duque-marin)

## En producción

El código de clientes es privado; los casos, sin nombres, están en [pabloduque.dev](https://pabloduque.dev).

- **Cliente del sector legal (Colombia):** del documento al dictamen. Amazon Textract y reglas
  deterministas para la póliza; Claude en Bedrock para la historia clínica, con una regla determinista
  que manda a revisión humana lo que no tiene un nexo claro. Orquestación por eventos en Terraform
  y frontend en React.
- **SaaS fiscal (España):** migración de un asistente con RAG a Frankfurt por el RGPD, con Terraform
  modular y multirregión, agentes de Bedrock actualizados y el almacén vectorial en S3 Vectors.

## Proyectos públicos

| Proyecto | Qué es | Resultado |
|---|---|---|
| [facturas-a-excel](https://github.com/pabdus/facturas-a-excel) | Facturas en PDF, escaneo o XML de la DIAN a JSON y Excel con validación contable. [Demo en AWS Lambda](https://rdd4yyol7clnebrcjjem4mdxmu0ubhqh.lambda-url.us-east-1.on.aws/). | 240 de 240 campos exactos con un LLM local y con Claude en Bedrock, frente a 67 % con reglas (20 facturas sintéticas, prompt congelado antes de medir). |
| [tfm-fdd-core](https://github.com/pabdus/tfm-fdd-core) | Paquete común del TFM (Máster en IA, UNIR): detección de fallos en el proceso Tennessee Eastman con PCA y DPCA (T², SPE). | Verificación ciega contra Yin et al. (2012) con la tolerancia fijada antes: 17 de 18 fallas idénticas y veredicto «no verificado» (la falla 19 se aparta 1 pp, con tolerancia de 0,5 pp). 643 pruebas. |
| [ctgan-adult-critical-evaluation](https://github.com/pabdus/ctgan-adult-critical-evaluation) | Evaluación de CTGAN en UCI Adult: fidelidad, utilidad (TSTR) y privacidad (DCR, ataque de inferencia de pertenencia). | El modelo base genera 62 % de valores imposibles que Wasserstein y JSD no detectan; un recorte de una línea los lleva a 0 % y conserva la utilidad. |
| [proyecto-02-obesidad-brfss](https://github.com/pabdus/proyecto-02-obesidad-brfss) | SMOTE frente a CTGAN con desbalance extremo (bajo peso: 1,52 %) en 289.693 registros del CDC BRFSS 2023. | CTGAN sin ganancia real: diferencias de 0,02 o menos en F1-macro con los tres clasificadores. |
| [proyecto-01-desigualdad-colombia](https://github.com/pabdus/proyecto-01-desigualdad-colombia) | Brechas urbano-rurales con microdatos del Censo DANE 2018 (15,4 M de personas, 5 departamentos). | En zona rural, el 14,9 % de las personas de 15 años o más no sabe leer ni escribir, frente al 2,3 % urbano: 6,6 veces más. Un script recalcula todas las cifras desde los microdatos. |

El sitio [pabloduque.dev](https://pabloduque.dev) también es público:
[portafolio](https://github.com/pabdus/portafolio), con S3 y CloudFront en Terraform y despliegue con
GitHub Actions por OIDC, sin claves guardadas.

## Stack

- **IA generativa y documentos:** Amazon Bedrock (Converse, Agents, Knowledge Bases, Prompt Management),
  Claude, Amazon Textract, S3 Vectors, Ollama, JSON Schema.
- **Nube e infraestructura:** Terraform, Lambda, EventBridge, SQS, DynamoDB, S3, CloudFront, Route 53,
  GitHub Actions con OIDC.
- **Datos y ML:** Python, SQL, pandas, scikit-learn, XGBoost, PyTorch.
- **Frontend:** React, Vite, GraphQL (Apollo), Testing Library.
- **Estadística:** control estadístico de procesos (PCA, T², SPE), Wilcoxon, Holm, TOST, SciPy, R.
- **Calidad:** pytest y Vitest con pruebas de mutación, SonarCloud.

## Formación

Máster en Inteligencia Artificial, UNIR (termina en febrero de 2027) · Maestría en Estadística
Aplicada, Universidad Cuauhtémoc (en curso) · Pregrado en Ciencia de Datos, Universidad Compensar
(en curso).

---

*In English:* AI engineer in Colombia (remote, UTC−5). I take generative AI to production on AWS and
measure with statistics whether it works. Case studies in Spanish and English at
[pabloduque.dev](https://pabloduque.dev).
