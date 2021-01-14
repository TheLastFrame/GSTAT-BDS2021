Materialien zur Lehrveranstaltung

## Grundlagen der Statistik

WS 20/21


### Vorbereitung zur LV

Wir werden in der LV einiges installieren. Sie können auch auf ihrem eigenen Laptop arbeiten,
dann müssen sie noch mehr installieren.

#### Software
Installieren sie folgende Software (es ist wichtig, dass sie die neuesten Versionen installieren):
(im Labor sollte das vorinstalliert sein)

R (von https://cran.r-project.org)
RStudio (von https://rstudio.com/products/rstudio/download/#download)
und für Windows auch Rtools (ebenfalls von https://cran.r-project.org)

Unter Windows tun sie dazu folgendes:

Laden sie folgende Dateien herunter:

  * https://cran.r-project.org/bin/windows/base/R-4.0.3-win.exe
  * https://download1.rstudio.org/desktop/windows/RStudio-1.3.1093.exe
 * https://cran.r-project.org/bin/windows/Rtools/rtools40-x86_64.exe
  * https://github.com/git-for-windows/git/releases/download/v2.30.0.windows.1/Git-2.30.0-64-bit.exe


Zur Installation gehen sie so vor

  * Führen sie das Installationsprogramm heruntergeladene `R-4.0.3-win.exe` aus   
  * Im Installationsdialog dieses Programm machen sie folgendes:   
    -  Customize Startup Options
		*  SDI (separate Windows)
		*  HTML Help
		*  Create a desktop shortcut
		*  Save version number in registry
		*  Associate R with .RData file 
	* Führen sie das Installationsprogramm `Rtools40.exe` aus und akzeptieren sie die Standard-Einstellungen
	* Führen sie das Installationsprogramm `RStudio-1.3.1093.exe` aus
	* Wenn die Installation fertig ist starten sie `RStudio` vom Start Menu.
	* Nachdem RStudio läuft erscheint ein Icon im Taskbar. Klicken sie auf das Icon und führen sie `Pin to Taskbar` aus.
  * Führen sie das Installationsprogramm `Git-2.30.0-64-bit.exe` aus und akzeptieren sie die Standardeinstellungen.
    
Die Installation der Programme ist jetzt abgeschlossen, aber es müssen noch einige Zusatzpakete in R bzw. RStudio installiert werden.

Kopieren sie dazu folgenden Code in das `Console`-Window von RStudio (und drücken sie, falls notwendig, RETURN):

```
pkgs_to_install <- c(
  "tidyverse",
  "magrittr",
  "ggmosaic",
  "ggforce",
  "ggExtra",
  "gridExtra",
  "ggthemes",
  "ggThemeAssist",
  "ggplot2movies",
  "ggmap",
  "ggrepel",
  "ggwordcloud",
  "broom",
  "tweenr",
  "maptools",
  "viridis",
  "egg",
  "scales",
  "sf",
  "sfheaders",
  "maptools",
  "rgeos",
  "pracma",
  "readxl",
  "writexl",
  "Dykstra",
  "quadprog",
  "devtools",
  "cowplot", 
  "flextable",
  "googleway", 
  "ggplot2", 
  "ggrepel", 
  "ggspatial", 
  "rworldmap", 
  "rworldxtra",
  "lwgeom",
  "rayshader",
  "shiny",
  "reprex",
  "datapasta",
  "tidytext",
  "lubridate",
  "Hmisc",
  "cartogram",
  "summarytools",
  "gganimate",
  "dplyrAssist",
  "rio",
  "csvy", 
  "fst", 
  "hexView", 
  "rmatio",
  "gifski",
  "png",
  "patchwork",
  "rtweet",
  "stationaRy",
  "curl",
  "ggiraph",
  "esquisse",
  "ggbeeswarm",
  "ggalluvial",
  "styler",
  "tidylog",
  "tidyr",
  "Rcpp",
  "RcppArmadillo",
  "rgl",
  "rglwidget",
  "readODS",
  "systemfonts",
  "xkcd",
  "plotly",
  "ggridges",
  "rtweet",
  "threejs",
  "gt"
)

for (pkg in pkgs_to_install){
if (!(pkg %in% rownames(installed.packages())))
install.packages(pkg)
}
```


Führen sie dann noch (in einem Command-Fenster) folgenden Befehl aus:   
`git config --global credential.helper wincred`




Wenn sie auf ihrem Rechner `TeX` noch nicht installiert haben, dann
führen sie auch folgenden Code aus:

```
install.packages("tinytex")
library(tinytex)
install_tinytex()
```


#### Maxima

Hilfreich für schnelle mathematische Zwischenrechnungen ist auch Maxima. Bitte istallieren sie das auch, falls sie es noch nicht installiert haben.

Die Versionen für ihr Betriebssystem finden sie hier:    
https://sourceforge.net/projects/maxima/files/

Die Windows-Version ist: https://sourceforge.net/projects/maxima/files/Maxima-Windows/5.44.0-Windows/maxima-clisp-sbcl-5.44.0-win64.exe/download


#### Notepad++

Sehr empfehlenswert unter Windows ist auch Notepad++

https://notepad-plus-plus.org/downloads/

#### Andere Betriebssysteme

Wenn sie Linux oder MacOS verwenden installieren sie bitte R (Version 4.0.3) und RStudio (Version 1.3.1093)
von den genannten Websites (es gibt dort auch Versionen für diese Betriebssysteme).    

Git müssen sie ebenfalls installieren. Zur Installation ziehen
sie das Internet zu Raten.     
Unter MacOS ist für solche Utilities die Installation von homebrew (https://brew.sh) sehr zu empfehlen.

Unter MaOS müssen Sie auch noch Xquartz von (https://www.xquartz.org) installieren.

### Spreadsheets

Auf Windows und MacOS sollten sie auch Microsoft Excel und Microsoft Word und/oder LibreOffice (https://www.libreoffice.org) installiert haben, auf Linux LibreOffice.


	
## Literaturempfehlungen zur LV

  * R for Data Science (https://r4ds.had.co.nz)
  * Online Statistics Education: An Interactive Multimedia Course of Study  (http://onlinestatbook.com)
  * Statistical Thinking for the 21st Century (http://thinkstats.org)
  * Fahrmeir et al.: Statistik - der Weg zur Datenanalyse (https://www.springer.com/gp/book/9783662503713#otherversion=9783662503720)
  * Cheatsheets for R and RStudio (https://www.rstudio.com/resources/cheatsheets/)
  * Advanced R (http://adv-r.had.co.nz)

  