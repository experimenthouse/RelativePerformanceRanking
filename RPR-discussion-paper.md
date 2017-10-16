# Relative performance ranking

## Summary

In sports such as Formula 1, the success of a driver depends on their performance as an individual and the performance of their equipment. Unlike other formula motor racing series such as Formula 2, Formula 1 does not use a single-make vehicle. The result is that Formula 1 drivers of considerable skill may be unable to overcome the technical limitations of their vehicles, and their ultimate points scored in a season will not reflect their potential. In this paper we discuss the possibility of devising a ranking system that makes allowance for the differences in performance, using Formula 1 as the example.

## Baseline factors

Each Formula 1 season consists of a number of teams, drivers and events. There may be up to 13 teams in any given season. Each team enters two cars per event, and may have up to four drivers per season, though most teams will have two drivers who compete in most or all events in a season. Events consist of a number of sessions: three free practice sessions, a qualifying session divided into three segments, and a race session. Free practice sessions are non-competitive.

Points are awarded to the drivers who finish the race session in the top ten: 25, 18, 15, 12, 10, 8, 6, 4, 2 or 1 points are awarded depending on where a driver finishes. Qualifying is used to determine the position of each driver on the starting grid. The driver who sets the fastest time in qualifying starts in pole position at the front. Other drivers line up in a staggered grid two cars wide following their qualifying order. Drivers may be given penalties that drop them a certain number of positions on the starting grid for breaches of technical and sporting regulations. Drivers' fastest lap times during the race session are also recorded.

A baseline ranking system could use the following factors:

1. Qualifying result
2. Race result
3. Fastest lap time

### Possible options for baseline ranking

The points system used in Formula 1 only awards points for the top ten drivers who finish a race session. These points are not spread in a linear fashion: the winning driver receives 25 points, and the 10th driver receives one point. This ignores the midfield drivers whose cars are simply incapable of breaking into top ten, and skews the results in favour of a first-place finish: a driver who finishes third in three races will receive 45 points, while a driver who finishes first in one race and fifth in two others will receive the same number of points.

A linear scoring system that divides points evenly between the drivers allows for a more accurate reflection of driver abilities. This could be calculated based on the number of entrants and finishing position like so:

_S = E - P_

In this, S is the score, E is the number of entrants and P is the finishing/qualifying/lap time position. If there are 26 drivers entered for an event, the driver who finishes first will receive 25 points, and the driver who finishes last will receive no points.

This approach has the advantage of being able to included results from multiple seasons. A driver who finishes first in a 26-entrant event has performed better than 25 other drivers; a driver who finishes first in a 20-entrant event has performed better than 19 other drivers.

## Retirement adjustments

A driver may fail to complete a session due to one of several factors:

- **Technical failures:** A problem with the vehicle that has required the driver to retire from the session.
- **Driver errors:** A retirement caused by a driver's own mistake or where the driver is wholly or predominantly to blame in accordance with a decision of the race stewards.
- **Collision damage:** A collision caused where another driver is wholly or predominantly to blame in accordance with a decision of the race stewards.
- **Racing incidents:** A collision where no driver is wholly or predominantly to blame in accordance with a decision of the race stewards.

In the case of a technical failure or collision damage, penalising the driver does not reflect the driver's culpability for the retirement. However, a driver error has some bearing on the judgment of the driver's skill. A racing incident sits somewhere in between these: while the driver is not wholly or predominantly responsible, they have at least contributed, and this should be taken into account.

In a qualifying session, each segment features fewer drivers than the previous segment. The final segment (Q3) always consists of 10 drivers, with equal numbers of the remaining drivers being eliminated in the first segment (Q1) and second segment (Q2). In a full grid of 26 cars, the slowest eight are eliminated in Q1 and the remaining cars repeat this in Q2, with another eight being eliminated. The remaining 10 drivers then compete in Q3.

If a driver retires during qualifying, they may still have set a time for qualifying: for example, a driver who makes it through to Q2 but retires without setting a time in Q2 will still have their Q1 qualifying time. If the driver has retired due to a technical failure and usually makes it through to Q3, in keeping with the no-penalty principle this should not affect their overall rank. Conversely, a driver who does not usually make it through to Q3 but does and subsequently retires should not have their achievement diminished. That is: if technical failures are compensated for, this should not result in a driver having a reduction in their qualifying result.

### Adjusting for retirements

In the event of a technical failure or collision damage, a driver could be awarded an average of the points received for sessions of the same type. This ensures the driver is not penalised for retirements that were out of their control. This could be done like so:

`_S = ( P / E ) * R_`

In this, S is the score, P is the number of points so far, E is the number of events completed, and R is the number of retirements. This means a driver whose average points scored was 10 would receive this for each race where they retired due to circumstances beyond their control.

In the event of a driver error, the driver should receive no points.

In the event of a driver error, the points awarded could be halved or otherwise divided, based on the average points awarded. Because no driver is wholly or predominantly to blame, it cannot be treated as collision damage or driver error. Each driver is deemed equally to blame. Whether the points should be divided by the number of drivers involved (rarely there are more than two drivers involved) is a difficult question, especially as more often than not two drivers collide and take out others with them. Perhaps those should be treated as victims of collision damage. Analysis of each incident would be required.

For example: in the 2017 Singapore Grand Prix, Max Verstappen was squeezed between Kimi Räikkönen on his left and Sebastian Vettel on his right. Vettel took an aggressive line, veering diagonally across the track. Verstappen then collided with Räikkönen who was attempting to overtake on Verstappen's left. Fernando Alonso was not involved in the initial collision, but a severely-damaged Räikkönen who was unable to control his car crashed into him. This incident was deemed a racing incident. In this situation, it seems that Verstappen, Räikkönen and Vettel each have some share of responsibility (the average points should perhaps be divided by three) while Alonso was not responsible (perhaps deserving full average points).

For qualifying adjustments, due to the segmented nature, the average points given should not be _lower_ than the position at which they retired. If a driver's average qualifying position is 15th, and they retire due to technical failure while sitting in 10th, their 10th place should stand. However, if the driver retires while sitting in 20th, this should be increased to 15th.

## Teammate adjustments

At most events drivers of the same team have identical or near-identical equipment, but may have adjustments made to their own requirements. This provides an opportunity for comparing the relative skills of drivers regardless of their equipment. A driver who outperforms his teammate should be rewarded, and the teammate who is outperformed should have a penalty applied.

### Calculating teammate adjustments

Adjusting for teammates' differences in performance could be done by averaging their points and increasing or decreasing each drivers' points according to how far above or below the average their result is. This could be done simply like so:

`_B = P - ( X + Y / 2 )_`

In this, B is the bonus received, P is the points of either driver, and X and Y are the points of the drivers. For example, if one driver receives 15 points and the other receives 5 points:

`_B = 15 - ( 15 + 5 / 2 ) = 15 - 10 = 5`(points increase)

`_B = 5 - ( 15 + 5 / 2 ) = 5 - 10 = -5` (points decrease)

## Starting grid and finishing positions

During a race, a driver has the opportunity to make up places: they may start seventh and finish third, for example. Drivers should be rewarded for the number of positions they have gained between the starting grid and the end of the race, and penalised for the number of positions they have lost. This can be done simply by awarding or deducting one point for each place difference:

`_B = S - F_`

In this, B is the bonus points, S is the starting position, and F is the finishing position.

## Summary of factors

1. Qualifying result relative to all other drivers.
2. Qualifying result relative to teammate.
3. Race result relative to all other drivers.
4. Race result relative to teammate.
5. Fastest lap relative to all other drivers.
6. Fastest lap relative to teammate.
7. Finishing position relative to starting position.
8. Technical failures.
9. Driver errors.
10. Collision damage.
11. Racing incidents.
