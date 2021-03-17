# LaTeX Annual Calendar
======================

## Introduction

This LaTeX calendar uses the [tikz-kalender](https://www.ctan.org/pkg/tikz-kalender) to generate a TeX based annual calendar with custom events.

## Get Started

The current year is given with the year parameter and event files are included with the events parameter in the TeX file.

```latex
\setup{
	paper=letter,
	print=true,
	year=2021,
	title={Annual calendar},
	showweeknumbers,
	titleColor=black,
	monthBGcolor=black,
	saturdayColor=blue!20,
	sundayColor=blue!40,
	eventColor=red,
	periodColor=gray!20,
	lang=american,
	events={events/Trash_2021,events/Recycling_2021,events/Holiday_2021,events/German_holidays_2021}
}
```

The event files are located in the events subfolder.

As example, the German and US Holidays and trash and recycling pickup schedule of 2021 are included as event files.

**Example for an event entry:**

`\event*{2021-10-11}{Columbus Day}[color=DeepSkyBlue]`

The first parameter is the event date, the next parameter is the event name and the last optional parameter is the background color of the event entry in the calendar.
