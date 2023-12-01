# Transcreva Áudios com OpenAI Whisper

[Open In Colab](https://user-images.githubusercontent.com/54370274/224839806-8720fb19-9c7d-46a2-8d7c-de3afb39c11f.svg)](https://colab.research.google.com/drive/1KnGFSofpxF5gbpwasQnOhg9JikVNblAg?usp=sharing)  

## Introdução
Este notebook utiliza o Whisper da OpenAI, um modelo avançado de reconhecimento de fala, para transcrever e traduzir arquivos de áudio.

## Configuração Inicial
1. Salve uma cópia do notebook no seu Google Drive a partir do Google Colab.
2. Abra o notebook no Google Drive, preferencialmente no Google Chrome.

## Etapas
### Etapa 1: Instalar o Whisper
```bash
!pip install git+https://github.com/openai/whisper.git
```

### Etapa 2: Instalar o ffmpeg
```bash
!sudo apt update && sudo apt install ffmpeg
```

### Etapa 3: Carregamento do Arquivo
Opções para upload do arquivo .mp3:
- Upload Direto: Use `files.upload()` no Colab.
- Upload Manual: Arraste e solte o arquivo na seção "Arquivos" do Colab.

### Etapa 4: Transcrever
Transcreva seu arquivo .mp3:
```bash
!whisper "nome_do_seu_arquivo.mp3" --model medium --language Portuguese
```

## Licença
Licença MIT. Veja `LICENSE` para mais detalhes.

## Créditos
- Tutorial traduzido por Thiago Borges.
- Direitos Autorais (c) 2022 Jason Boog.
