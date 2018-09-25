<!--

author:   André Dietrich, Sebastian Zug
email:    andre.dietrich@ovgu.de, sebastian.zug@ovgu.de
version:  1.0.0
language: de
narrator: Deutsch Female

script:   https://cdn.rawgit.com/davidedc/Algebrite/master/dist/algebrite.bundle-for-browser.js

script: https://cdn.jsdelivr.net/chartist.js/latest/chartist.min.js

link: https://cdn.jsdelivr.net/chartist.js/latest/chartist.min.css

@eval:    <script> Algebrite.run(`@input`) </script>

-->

# Netzwerktreffen2018

Demo: Netzwerktreffen Hochschulforum Digitalisierung 2018

https://LiaScript.github.io

Kurs auf Github: https://github.com/liaScript/Netzwerktreffen2018

Kurs auf LiaScript: https://liascript.github.io/course/?https://raw.githubusercontent.com/liaScript/Netzwerktreffen2018/master/README.md#1

## Einleitung

Dieser Workshop stellt einige der Features von LiaScript im Rahmen des Netzwerktreffens "Hochschulforum Digitalisierung" vor.

## Das eLab Projekt

!?[YouTube](https://www.youtube.com/embed/bICfKRyKTwE)

## Algebrite

http://algebrite.org/

```
100!
```
@eval

```
factor(100!)
```
@eval

```
simplify(cos(x)^2 + sin(x)^2)
simplify(a*b+a*c)
simplify(n!/(n+1)!)
```
@eval


## Bilder

![Cosinus](img/Cosine.png)

## ASCII - Art




      |              *
    y |             * *
    - |
    A |            *   *
    c |  r  r  r  r  r  r  r  r  r
    h |           *     *
    s |          *       *
    e |        *           *
      |  * *                   * *
      +---------------------------
      0         x-Achse         10

## Javascript

https://gionkunz.github.io/chartist-js/

```yaml
{
  labels: [1, 2, 3, 4, 5, 6, 7, 8],
  series: [
    [1, 2, 3, 1, -2, 0, 1, 0],
    [-2, -1, -2, -1, -2.5, -1, -2, -1],
    [0, 0, 0, 1, 2, 2.5, 2, 1],
    [2.5, 2, 1, 0.5, 1, 0.5, -1, -2.5]
  ]
}
```
<script>
new Chartist.Line('#chart', @input, {
  high: 3,
  low: -3,
  showArea: true,
  showLine: false,
  showPoint: false,
  fullWidth: true,
  axisX: {
    showLabel: false,
    showGrid: false
  }
});
</script>

<div class="ct-chart ct-golden-section" id="chart"></div>
