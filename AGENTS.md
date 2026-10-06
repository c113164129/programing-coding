# AGENTS.md

- 語言：Python。套件一律用 conda 管理，不要用 `pip install`、venv 或 poetry。
- Conda 環境：`iem_python`（已驗證：`C:\Users\user\anaconda3\envs\iem_python`，Python 3.12.13）。執行一律用 `conda run -n iem_python ...`，例如 `conda run -n iem_python python <script>.py`、`conda run -n iem_python pytest <test>`。
- 本機 conda 主程式在 `C:\Users\user\anaconda3\Scripts\conda.exe`，且不在本工作階段的 `PATH` 上。若 `conda` 指令找不到，用完整路徑呼叫。
- Repo 狀態：greenfield。`README.md` 只是佔位符；尚無原始碼、manifest、lockfile 或 build/test/lint 設定。`README.md` 之外僅有 `.gitignore`（GitHub Python 範本）與 `.git/`。
- 尚無已驗證的 build、test、lint、typecheck 指令。新增設定後以可執行的設定檔為準，不要臆測指令。
- Shell 為 Windows PowerShell。避免 POSIX-only 指令（`head`、`ls -la`、heredoc 寫檔）；檔案操作優先用 `read`/`edit`/`write` 工具。
