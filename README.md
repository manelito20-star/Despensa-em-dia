## 🥫 Despensa Em Dia

**Despensa Em Dia** é uma aplicação Android moderna desenvolvida em **Jetpack Compose** (Material 3) com o objetivo de otimizar a gestão de stock de produtos alimentares e de limpeza em casa, combater o desperdício alimentar e simplificar as compras de supermercado.

---

## 🚀 Funcionalidades Principais

### 1. 📦 Inventário Inteligente
- **Adicionar por Câmara (Código de Barras):** Leitor de códigos de barras integrado em tempo real com **CameraX** e **ML Kit Barcode Scanning** (inclui controlo de lanterna para armários escuros).
- **Consulta Automática na Internet:** Ao ler um código de barras, a aplicação consulta automaticamente a base de dados pública do *Open Food Facts* para preencher o nome e a categoria do produto.
- **Gestão de Lotes e Validades:** Controlo de múltiplas embalagens e datas de validade independentes para cada produto.
- **Quantidade Ideal vs. Quantidade Atual:** Definição da quantidade ideal desejada em stock para cada artigo. Quando o stock desce abaixo do ideal, o sistema assinala automaticamente e calcula quantas unidades faltam comprar.
- **Consumo Rápido (`-` / `+`):** Botões diretos para retirar ou adicionar unidades à medida que consome os produtos.
- **Alertas de Validade & Stock:** Avisos visuais e notificações automáticas em segundo plano (*WorkManager*) para produtos prestes a expirar ou em falta.
- **Lista de Compras Automática:** Gera uma lista com base nos produtos em falta e permite **exportar e partilhar em PDF** instantaneamente via WhatsApp, E-mail, etc.

### 2. 🏷️ Etiquetagem & Organização (Kaizen / 5S)
- **Guia de Organização:** Página informativa integrada baseada na metodologia *Kaizen* e *5S* para arrumação inteligente de prateleiras (zonas por frequência de uso, separação de produtos de limpeza, regra FIFO).
- **Kits Rápidos e Etiquetas Manuais:** Seleção de pacotes predefinidos ou criação de texto personalizado para etiquetas.
- **Geração de Etiquetas em PDF:** Criação automática de um documento PDF com grelha de etiquetas finas e compactas (com linhas de corte), prontas a imprimir e colar nas prateleiras.

### 3. ⚙️ Definições e Alertas
- **Configuração de Validade:** Escolha da antecedência dos alertas de validade (5 dias, 15 dias ou 1 mês).
- **Configuração de Limiar de Stock:** Definição dos critérios de alerta de quantidade.

---

## 📱 Tecnologias Utilizadas
- **Kotlin** & **Jetpack Compose** (Material 3)
- **CameraX** & **Google ML Kit** (Leitura de códigos de barras)
- **AndroidX WorkManager** (Notificações e tarefas em segundo plano)
- **Android PdfDocument** (Geração nativa de PDFs para etiquetas e listas de compras)
- **Coroutines & Flow** (Processamento assíncrono)

---

## 📄 Licença
Projeto desenvolvido para teste, otimização e gestão doméstica de despensas.
