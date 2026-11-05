# Git практикалық тапсырмалар №1–4

**Орындаған:** Ембергенов Қазбек  
**Репозиторий:** https://github.com/k9121110-stack/kazbek

Бұл файл «Git нұсқаулық.pdf» құжатының 12-бөліміндегі №1–4 практикалық тапсырмалардың орындалуын қысқаша сипаттайды.

## №1. Git негіздері
**Талаптар:** Git орнату; автордың атын және email-ін баптау; жеке репозиторий, README.md және өзің туралы үш сөйлем; кемінде үш commit; git log --oneline.

**Нәтиже:** Windows-та Git 2.56.0.windows.4 жұмыс істейді. Автор аты мен email бапталған. README.md жасалған, үш сөйлем енгізілген және бірнеше commit бар. `git log --oneline` CMD-де тексерілді.

- [README.md](README.md)
- [Commit тарихы](../../commits/main)

## №2. .gitignore және өзгерісті болдырмау
**Талаптар:** .env жасап, .gitignore-ға енгізу; файлдың git status ішінде көрінбеуін тексеру; өзгерген файлды git restore арқылы қайтару.

**Нәтиже:** .gitignore ішінде `.env` тіркелген. CMD-де `git check-ignore .env` нәтижесі `.env` болды, `git status` оны көрсетпеді. README.md уақытша өзгертіліп, `git restore README.md` арқылы қалпына келтірілді; соңында `working tree clean` шықты.

- [.gitignore](.gitignore)
- **Ескерту:** .env құпия/локал файл ретінде GitHub-қа жүктелмейді; тексеру CMD-де орындалды.

## №3. Тармақтар мен конфликт
**Талаптар:** feature-hobbies тармағын ашу, hobbies.md жасау, main-ге біріктіру; feature-title тармағында README.md бірінші жолын main-нен өзгеше өңдеп конфликт жасау; конфликтті шешу.

**Нәтиже:** feature-hobbies тармағында hobbies.md қосылды және PR №1 арқылы main-ге біріктірілді. feature-title және main-де README.md тақырыбы әртүрлі өзгертіліп, GitHub PR №2-де конфликт анықталды; кейін шешіліп, біріктірілді.

- [hobbies.md](hobbies.md)
- [Pull Request №1](../../pull/1)
- [Pull Request №2](../../pull/2)

## №4. GitHub: SSH, push және pull
**Талаптар:** SSH кілтін орнату, `ssh -T git@github.com` тексеру; репозиторийді GitHub-қа push жасау; README-ді GitHub-та өзгертіп, жергілікті компьютерге pull жасау.

**Нәтиже:** Windows компьютерінде SSH ашық кілті GitHub аккаунтына қосылған. `ssh -T git@github.com` нәтижесі: `Hi k9121110-stack! You've successfully authenticated`. `practice.txt` файлы жеке commit арқылы `git push -u origin main` көмегімен жіберілді (`233d988`). GitHub-та README жаңартылған соң `git pull origin main` арқылы `7c46d24` commit жергілікті компьютерге алынды. Соңғы `git status`: `working tree clean`.

- [practice.txt](practice.txt)
- [README.md](README.md)
- [Commit тарихы](../../commits/main)

## Тапсыру
GitHub репозиторийі: https://github.com/k9121110-stack/kazbek

**Нақтылау:** Нұсқаулықтағы мысал репозиторий атауы `about-me`; тәжірибе `kazbek` репозиторийінде орындалған. CMD-де орындалған жергілікті әрекеттер сайттағы commit тарихынан тікелей көрінбейді, олардың дәлелі - тексеру кезінде түсірілген скриншоттар.
