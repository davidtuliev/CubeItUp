# CubeItUp

ПРОЕКТНА ЗАДАЧА ПО ВИЗУЕЛНО ПРОГРАМИРАЊЕ 
ИМЕ НА ПРОЕКТ: CubeItUp
ЧЛЕНОВИ НА ТИМОТ: Никола Дургутев 185041, Давид Тулиев 181531

1.ОПИС
Апликацијата која ја направивме игра која ја реализиравме  со помош на развојната околина за видео игри Unity Engine. 
Играта претставува платформер во кој целта е минување на левели со избегнување на препреки

2.КАКО СЕ ИГРА

Со притискање на копчето А се мрда лево, а со копчето D се мрда десно. Низ левелот има препреки коишто прогресивно се потешки со текот на иргање. 
Играчот контролира топче кое се движи по платформа, одејќи премногу десно или пемногу лево предизвикува топчето да падне од платформата и се рестартира левелот,
исто така и при допирање на препреката се рестартира левелот. На горната страна од екранот има скор кој со прогресот на левелот се зголемува, почнувајќи од 0.
Има 7 левела и при поминување на сите на екранот се прикажува текст “Congratulations”.
Исто така низ левелот има Power-ups кои кога ке поминеш врз нив го убрзуваат движењето лево и десно, олеснувајќи го левелот.
На почетокот при уклучувањето на играта има Welcome секција која е доста едноставна. Има само едно копче play и инструкции за како се игра. На крајот има credits.

3. КЛАСИ И НИВНА УЛОГА

PlayerMovement класата е задолжено за движењето. Ако стиснатото копче е d, движењето е на десно додека на лево се движе со копчето а,
ова се постигнува само со додавање на  “-” на променливата задолжена за странично движење,со која е овозможено движењето лево и десно.
Брзината за движење напред е константно 200.

CameraMechanics класата ги чува позицијата на играчот и координатите на кои треба да се придржува камерата.

Во collision  класата се гледа дали има контакт со некоја од препреките. Има една променлива move. Колизијата се проверува со if циклусот каде ако тагот 
е “Obstacle” променливата move станува false и играта завршува. Доколку пак ако тагор е од тип “Powerup” се зголемува брзината со која се движиме напред, 
а исто така има и зголемување на брзината за лево и десно.
Доколку тагот е од тип “Sidepowerup” има зголемување само на брзината за лево и десно.

levelcomplete класата се активира кога завршува левелот и се лоадира следниот левел со зголемување на buildIndex  за еден.


![alt text](http://url/to/img.png)

