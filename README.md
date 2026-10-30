# Escola Bitcoin

Site https://escolabitcoin.com com duas abas: **Tutoriais** (playlist *Tutoriais e passo-a-passos* do [canal no YouTube](https://www.youtube.com/@BitcoineLiberdade)) e **Mentoria e Consultoria**.

Playlist: https://www.youtube.com/playlist?list=PL1TShuYSNH-t3VCQK-YwCfdtMS2iO_ybV

## Como se atualiza sozinha

- O player embutido na página lê a playlist direto do YouTube (sempre atual).
- Um GitHub Action (`.github/workflows/atualizar.yml`) roda a cada 3 horas, executa `scripts/update_playlist.py` e, se entrou ou saiu vídeo, atualiza `videos.json` com um commit automático.
- Para forçar agora: aba **Actions → Atualizar playlist → Run workflow**.

Para rodar localmente: `python scripts/update_playlist.py` (sem dependências, sem chave de API).
