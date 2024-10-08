## Содержание

Ссылка на статью - <https://imbicile.pp.ru/podsvetka-v-bash/>

1. .bashrc - Конфигурация bash
2. shell_color - Файл установки
3. shell_color_ansible - Файл установки стиля из роли ansible

## Установка

```bash
wget https://raw.githubusercontent.com/alivalutor/shell_colors/master/shell_color
chmod +x shell_color
./shell_color
rm shell_color
```

## Установка подсветки nanorc из [imbicile.nano](https://github.com/imbicile/imbicile.nano)

```bash
wget https://raw.githubusercontent.com/alivalutor/shell_colors/master/nanorc
chmod +x nanorc
./nanorc
rm nanorc
```

## Установить всё одной командой

```bash
wget https://raw.githubusercontent.com/alivalutor/shell_colors/master/shell_color && chmod +x shell_color && ./shell_color && rm shell_color && wget https://raw.githubusercontent.com/alivalutor/shell_colors/master/nanorc && chmod +x nanorc && ./nanorc && rm nanorc
```

## Установить всё одной командой с доп.пакетами на сервер VDS с Debian 12

```bash
apt install nethogs iptraf locales chrony exa curl htop iftop atop duf bwm-ng && echo "ru_RU.UTF-8 UTF-8" | tee -a /etc/locale.gen && locale-gen ru_RU.UTF-8 && update-locale LANG=ru_RU.UTF-8 && wget https://raw.githubusercontent.com/alivalutor/shell_colors/master/shell_color && chmod +x shell_color && ./shell_color && rm shell_color && wget https://raw.githubusercontent.com/alivalutor/shell_colors/master/nanorc && chmod +x nanorc && ./nanorc && rm nanorc && systemctl enable chrony && timedatectl set-timezone Europe/Moscow
```

## Для автоматизации установки лучше использовать ansible [imbicile.environment](https://github.com/imbicile/imbicile.environment)

## Ссылки на источники

1. Файл подсветки ls - <https://github.com/trapd00r/LS_COLORS>
2. Список цветов bash - <https://wiki.archlinux.org/index.php/Bash/Prompt_customization_(%D0%A0%D1%83%D1%81%D1%81%D0%BA%D0%B8%D0%B9)>
3. Готовые конфигурации bash - <http://dotshare.it/category/shells/bash/>
4. Роль для установки через ansible - <https://github.com/imbicile/imbicile.environment>
