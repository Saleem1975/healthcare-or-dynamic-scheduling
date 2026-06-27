# Executive Summary

## Project title

**CNN-Based Dynamic Operating Room Scheduling for Healthcare Operations Improvement**

## Summary

This project demonstrates how machine learning can support operating room scheduling by predicting the remaining intra-surgical time from laparoscopic surgery videos. The approach uses a Convolutional Neural Network (CNN) to detect the end of Gallbladder Dissection Phase 4 during laparoscopic cholecystectomy procedures. Detecting this phase is operationally important because it provides a real-time signal that the surgery is nearing completion and that the next patient, anesthesia team, and operating room preparation activities can be coordinated more effectively.

## Business problem

Operating room schedules are difficult to manage because surgery durations vary across patients and procedures. Traditional static schedules often rely on fixed historical averages. When real surgeries deviate from those averages, hospitals may experience patient waiting time, operating room idle time, delayed starts, staff coordination problems, and lower overall utilization.

## Analytical solution

The proposed solution uses surgical video frames as real-time input. The CNN model classifies whether a frame indicates the end of Phase 4. Once the end of Phase 4 is detected, the schedule can be updated dynamically. This creates a data-driven trigger for operational decision-making rather than relying only on fixed historical timing assumptions.

## Reported impact

In the ten-surgery test schedule, the CNN-based dynamic scheduling method:

- Reduced total patient waiting time from **103 minutes to 13 minutes**
- Achieved an **87.3% reduction** in patient waiting time
- Reduced operating room idle time from **28 minutes to 0 minutes**

## Strategic value

This project is relevant to healthcare operations transformation because it connects artificial intelligence with measurable process improvement. It demonstrates how computer vision and predictive analytics can help hospitals improve scheduling accuracy, resource utilization, patient flow, and service efficiency.
