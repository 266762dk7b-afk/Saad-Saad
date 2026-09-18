telnet gameboy.live 1989git clone https://github.com/HFO4/gameboy.live.git
cd gameboy.live
go build -o gbdotlive main.goUsage of gbdotlive:
  -G    Play specific game in Fyne GUI mode
  -S    Start a static image cloud-gaming server
  -c config
        Set the game option list config file path
  -d    Use Debugger in GUI mode
  -f FPS
        Set the FPS in GUI mode (default 60)
  -g    Play specific game in GUI mode (default true)
  -h    This help
  -m    Turn on sound in GUI mode (default true)
  -p port
        Set the port for the cloud-gaming server (default 1989)
  -r ROM
        Set ROM file path to be played in GUI mode
  -s    Start a cloud-gaming server
gbdotlive -G -r "Tetris.gb" [{
	"Title": "Tetris",
	"Path": "test.gb"
}, {
	"Title": "Dr. Mario",
	"Path": "Dr. Mario (JU) (V1.1).gb"
}, {
	"Title": "Legend of Zelda - Link's Awakening",
	"Path": "Legend of Zelda, The - Link's Awakening (U) (V1.2) [!].gb"
}]
[{
	"Title": "Tetris",
	"Path": "test.gb"
}, {
	"Title": "Dr. Mario",
	"Path": "Dr. Mario (JU) (V1.1).gb"
}, {
	[{
	"Title": "Tetris",
	"Path": "test.gb"
}, {
	"Title": "Dr. Mario",
	"Path": "Dr. Mario (JU) (V1.1).gb"
}, {
	"Title": "Legend of Zelda - Link's Awakening",
	"Path": "Legend of Zelda, The - Link's Awakening (U) (V1.2) [!].gb"
}]
gbdotlive -s -c "gamelist.json"
2019/04/30 21:27:56 Listen port: 1989 
