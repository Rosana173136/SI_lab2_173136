# SI_lab2_173136


### Control Flow Graph
Фотографија од control flow graph-ot https://imgur.com/a/ztu9jgQ

3.1 Иницијализација на променливата i во рамката 

3.2 Услов во рамката (i < timesList.size())   

3.3 Зголемување на променливата i во рамката

### Цикломаткса комплексност
Во овој граф имаме 24 јазли и 34 ребра па зато цикломатската комплексност е: (34-24)+2 = 8 исто така овој резултат можеме да го добиеме и со броење на предикатни јазли(7) и додавање 1: 7+1 = 8.

### Тест случаи според критериумот Multicond
Имаме 4 if услови со multiple conditions:
if (hr < 0 || hr > 24)
T|T (hr = mins = sec= )
T|F (hr = mins = sec= )
F|T (hr = mins = sec= )
F|F(hr = mins = sec= )

if (min < 0 || min > 59)
T|T (hr = mins = sec= )
T|F (hr = mins = sec= )
F|T (hr = mins = sec= )
F|F (hr = mins = sec= )

if (sec >= 0 && sec <= 59)
T&T (hr = mins = sec= )
T&F (hr = mins = sec= )
F&T (hr = mins = sec= )
F&F (hr = mins = sec= )

if (hr == 24 && min == 0 && sec == 0)
T&T&T (hr = mins = sec= )
T&T&F (hr = mins = sec= )
T&F&T (hr = mins = sec= )
T&F&F (hr = mins = sec= )
F&T&T (hr = mins = sec= )
F&T&F (hr = mins = sec= )
F&F&T (hr = mins = sec= )
F&F&F (hr = mins = sec= )


### Тест случаи според критериумот Every branch


