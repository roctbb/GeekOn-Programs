### Dota 2

Вы слышали об игре Dota 2? В ней есть три дороги, соединяющие базы противников. Представим, что все игроки заняты борьбой между собой, и вся игра зависит от крипов - игроков ИИ, выбегающих на каждую дорогу в каждый момент времени. 

Количество крипов, выбегающих из каждой базы на каждую дорогу в каждый момент времени последовательно вводиться с клавиатуры. Силы всех крипов одинаковые, два крипа противоположных команд при встрече погибают.

Если на дороге остается более 10 крипов одной команды - эта команда побеждает.

<table>
<tr><td>Ввод</td><td>Вывод</td></tr>
<tr><td>
1 1 1 <b>1 1 1</b> <i>(все погибли)</i><br>
1 2 1 <b>2 1 2</b> <i>(на каждой дорожке по 1)</i><br>
2 1 2 <b>1 2 1</b> <i>(снова никого не осталось)</i><br>
10 0 0 <b>0 1 1</b> <i>(10 на первой - еще играем)</i><br>
1 0 0 <b>0 0 0</b> <i>(11 - победа 1 команды)</i><br>
</td>
<td>Radient win</td>
</tr>
<tr><td>
0 0 0 <b>0 11 0</b>
</td><td>Dire win</td></tr>
 <tr><td>
11 11 0 <b>0 0 11</b>
</td><td>Draw</td></tr>
</table>

