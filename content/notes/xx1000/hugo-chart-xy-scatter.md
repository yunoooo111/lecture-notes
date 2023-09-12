---
title: "hugo-chart xy scatter"
date: 2023-09-13T05:44:00+08:00
authors: ['Sparisoma Viridi']
tags: ['xx1000']
draft: false
math: true
url: "0044"
---
{{< toc >}}

## result
{{< chart 90 300 >}}
{
  type: 'scatter',
  data:
  {
    datasets:
    [
      {
        label: 'wander = 0',
        pointRadius: 4,
        pointBackgroundColor: "rgba(255,0,0,0.5)",
        showLine: true,
        fill: false,
        borderColor: "rgba(255,0,0,0.5)",
        lineTension: 0.0,
        data:
        [
          {x: 10, y:0.020},
          {x: 20, y:0.030},
          {x: 30, y:0.095},
          {x: 40, y:0.155},
          {x: 50, y:0.175},
          {x: 60, y:0.220},
          {x: 70, y:0.240}
        ]
      },
      {
        label: 'wander = 10',
        pointRadius: 4,
        pointBackgroundColor: "rgba(0,0,255,0.5)",
        showLine: true,
        fill: false,
        borderColor: "rgba(0,0,255,0.5)",
        lineTension: 0.0,
        data:
        [
          {x: 10, y:0.025},
          {x: 20, y:0.075},
          {x: 30, y:0.125},
          {x: 40, y:0.190},
          {x: 50, y:0.190},
          {x: 60, y:0.175}
        ]
      },
    ]
  },
  options:
  {
    maintainAspectRatio: true,
    scales: {
      yAxes: [
        {
          ticks: {
            beginAtZero: true
          }
        }
      ]
    }
  }
}
{{< /chart >}}


## refs
+ hugo-chat ([Shen et al., 2023](https://github.com/shen-yu/hugo-chart))


## test
```md
{{</* chart 90 200 */>}}
{
    type: 'bar',
    data: {
        labels: ['Red', 'Blue', 'Yellow', 'Green', 'Purple', 'Orange'],
        datasets: [{
            label: 'Bar Chart',
            data: [12, 19, 18, 16, 13, 14],
            backgroundColor: [
                'rgba(255, 99, 132, 0.2)',
                'rgba(54, 162, 235, 0.2)',
                'rgba(255, 206, 86, 0.2)',
                'rgba(75, 192, 192, 0.2)',
                'rgba(153, 102, 255, 0.2)',
                'rgba(255, 159, 64, 0.2)'
            ],
            borderColor: [
                'rgba(255, 99, 132, 1)',
                'rgba(54, 162, 235, 1)',
                'rgba(255, 206, 86, 1)',
                'rgba(75, 192, 192, 1)',
                'rgba(153, 102, 255, 1)',
                'rgba(255, 159, 64, 1)'
            ],
            borderWidth: 1
        }]
    },
    options: {
        maintainAspectRatio: false,
        scales: {
            yAxes: [{
                ticks: {
                    beginAtZero: true
                }
            }]
        }
    }
}
{{</* /chart */>}}
```
