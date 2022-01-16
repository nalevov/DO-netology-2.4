й# DO-netology-2.4
1. Полный хэш коммита aefea:

   aefead2207ef7e2aa5dc81a34aedf0cad4c32545 , комментарий   Update CHANGELOG.md

   получен командой git show aefea

2. Коммит 85024d3 соответствует тэгу v0.12.23 

   получен командой git show 85024d3

3. У коммита 2 родителей, их хэши: 56cd7859e05c36c06b56d013b55a252d0bb7e158 и 9ea88f22fc6269854151c571162c5bcf958bee2b
   
   получен коммандами git show b8d720^1 и git show b8d720^2

4. Между тегами v0.12.23 и v0.12.24 были сделаны следующие коммиты:
   
   33ff1c03b (tag: v0.12.24) v0.12.24
   
   b14b74c49 [Website] vmc provider links
   
   3f235065b Update CHANGELOG.md 
   
   6ae64e247 registry: Fix panic when server is unreachable
   
   5c619ca1b website: Remove links to the getting started guide's old location
   
   06275647e Update CHANGELOG.md
  
   d5f9411f5 command: Fix bug when using terraform login on Windows
   
   4b6d06cc5 Update CHANGELOG.md

   dd01a3507 Update CHANGELOG.md

   225466bc3 Cleanup after v0.12.23 release

   получен командой git show v0.12.23…v0.12.24 --oneline --no-patch
   
5. Функция func providerSource была добавлена в коммите: 

   8c928e835 main: Consult local directories as potential mirrors of providers

   получен командой git log -S 'func providerSource', выбираем первый коммит
   
   или коммандой git log -S 'func providerSource(' --pretty=format:'%h, %an, %ad, %s'


6. Вначале вводим git grep -p 'globalPluginDirs'


   затем команду git log -L:globalPluginDirs:plugins.go --oneline --no-patch

   получаем, что функция globalPluginDirs изменялась в следующих коммитах:

   78b122055 Remove config.go and update things using its aliases

   52dbf9483 keep .terraform.d/plugins for discovery

   41ab0aef7 Add missing OS_ARCH dir to global plugin paths

   66ebff90c move some more plugin search path logic to command

   8364383c3 Push plugin discovery down into command package 

7. Автором функции является Martin Atkins <mart@degeneration.co.uk>
   
   получена вводом команды git log -SsynchronizedWriters и выбором первого коммита
