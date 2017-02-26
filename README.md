# XOServer
Methods
\\server/?method=start&human={<int 0|1>} 
return json {
  id : <int>, 
  human : <int 0|1>, 
  symbol : <string 'x'|'o'>
}
\\server/?method=find 
return json {
  id : <int>
 }
\\server/?method=state&id={<int>} 
return json {
timetoclose : <int>, 
filled : <int 0|1>,
expected : <string 'x'|'o'>, 
state:[
    [<string ''|'x'|'o'>,<string ''|'x'|'o'>, <string ''|'x'|'o'>],
    [<string ''|'x'|'o'>,<string ''|'x'|'o'>, <string ''|'x'|'o'>],
    [<string ''|'x'|'o'>,<string ''|'x'|'o'>, <string ''|'x'|'o'>]
  ]
}
\\server/?method=move&id={<int>}&x={<int>}&y={<int>}
json {
win: <string 'x'|'o'>,
end: <int 0|1>,
timetoclose : <int>, 
filled : <int 0|1>,
expected : <string 'x'|'o'>, 
state:[
    [<string ''|'x'|'o'>,<string ''|'x'|'o'>, <string ''|'x'|'o'>],
    [<string ''|'x'|'o'>,<string ''|'x'|'o'>, <string ''|'x'|'o'>],
    [<string ''|'x'|'o'>,<string ''|'x'|'o'>, <string ''|'x'|'o'>]
  ]
}
