# XOServer
Methods<br />
\\server/?method=start&human={<int 0|1>} <br />
return json {<br />
  id : <int>, <br />
  human : <int 0|1>, <br />
  symbol : <string 'x'|'o'><br />
}<br />
\\server/?method=find <br />
return json {<br />
  id : <int><br />
 }<br />
\\server/?method=state&id={<int>} <br />
return json {<br />
timetoclose : <int>, <br />
filled : <int 0|1>,<br />
expected : <string 'x'|'o'>, <br />
state:[<br />
    [<string ''|'x'|'o'>,<string ''|'x'|'o'>, <string ''|'x'|'o'>],<br />
    [<string ''|'x'|'o'>,<string ''|'x'|'o'>, <string ''|'x'|'o'>],<br />
    [<string ''|'x'|'o'>,<string ''|'x'|'o'>, <string ''|'x'|'o'>]<br />
  ]<br />
}<br />
\\server/?method=move&id={<int>}&x={<int>}&y={<int>}<br />
json {<br />
win: <string 'x'|'o'>,<br />
end: <int 0|1>,<br />
timetoclose : <int>, <br />
filled : <int 0|1>,<br />
expected : <string 'x'|'o'>, <br />
state:[<br />
    [<string ''|'x'|'o'>,<string ''|'x'|'o'>, <string ''|'x'|'o'>],<br />
    [<string ''|'x'|'o'>,<string ''|'x'|'o'>, <string ''|'x'|'o'>],<br />
    [<string ''|'x'|'o'>,<string ''|'x'|'o'>, <string ''|'x'|'o'>]<br />
  ]<br />
}<br />
