# XOServer
Methods<br />
http://test.local/?method=start&human={<int 0|1>} return json {id : <int>, human : <int 0|1>, symbol : <string 'x'|'o'>}
http://test.local/?method=find return json {id : <int>}
http://test.local/?method=state&id={<int>} return json {timetoclose : <int>, filled : <int 0|1>, expected : <string 'x'|'o'>, state:[[<string ''|'x'|'o'>,<string ''|'x'|'o'>, <string ''|'x'|'o'>],[<string ''|'x'|'o'>,<string ''|'x'|'o'>, <string ''|'x'|'o'>],[<string ''|'x'|'o'>,<string ''|'x'|'o'>, <string ''|'x'|'o'>]}
http://test.local/?method=move&id={<int>}&x={<int>}&y={<int>} return json {timetoclose : <int>, filled : <int 0|1>, expected : <string 'x'|'o'>, state:[[<string ''|'x'|'o'>,<string ''|'x'|'o'>, <string ''|'x'|'o'>],[<string ''|'x'|'o'>,<string ''|'x'|'o'>, <string ''|'x'|'o'>],[<string ''|'x'|'o'>,<string ''|'x'|'o'>, <string ''|'x'|'o'>]}