# .config/conky/conky.conf

```
conky.config = {
out_to_console = true,
out_to_x = false,
background = false,
update_interval = 0.0166,
total_run_times = 0,
use_spacer = 'left',
};
conky.text = [[
${cpu cpu0}%  ${loadavg 1} :: ${acpitemp}c :: ${freq_g}Ghz :: ${battery_percent BAT0}%:${battery_time BAT0} :: $memperc% ($mem) :: ${downspeed wlp0s20f3}/s ${upspeed wlp0s20f3}/s :: ${exec amixer -c 0 get Master | grep Mono: | cut -d " " -f6 | sed 's/^\[\(.*\)\]$/\1/'} :: ${time %a %b %d %H:%M:%S}
]];
```
