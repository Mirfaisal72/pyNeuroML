Channel information
===================
    
<p style="font-family:arial">${info}</p>

<table>
#foreach ($channel in $channels)##
    <tr>
<td width="120px">
            <p style="font-size:70%;font-family:arial"><b>${channel.id}</b><br/>
            <a href="../${channel.file}">${channel.file}</a><br/><br/>
            Ion: ${channel.species}<br/><br/>
            ${channel.expression}<br/><br/>
            ${channel.notes}<br/></p>
</td>
<td>
<a href="${channel.id}.inf.png"><img alt="${channel.id} steady state" src="${channel.id}.inf.png" height="220"/></a>
</td>
<td>
<a href="${channel.id}.tau.png"><img alt="${channel.id} time course" src="${channel.id}.tau.png" height="220"/></a>
</td>
</tr>
#end##   
</table>
