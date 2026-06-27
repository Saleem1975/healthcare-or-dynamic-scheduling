# Business Impact

## Operational problem

Operating room scheduling is a high-impact healthcare operations problem. Inefficient schedules can create waiting patients, idle operating rooms, delayed anesthesia preparation, inefficient staff utilization, and downstream disruption across the surgical day.

The traditional static scheduling method used in the paper assumed:

- 40 minutes as the average surgery duration
- 45 minutes for cleaning and preparation of the operating room

This fixed-time approach does not account for real-time variability in surgical progress.

## Dynamic scheduling value

The CNN-based method detects the end of Phase 4 and uses that prediction as a signal to update the schedule. This enables staff to prepare for the next patient in a more timely and coordinated manner.

## Reported performance improvement

The ten-surgery schedule comparison showed:

| Metric | Traditional static scheduling | CNN-based dynamic scheduling | Improvement |
|---|---:|---:|---:|
| Total patient waiting time | 103 min | 13 min | 87.3% reduction |
| Total operating room idle time | 28 min | 0 min | Eliminated |
| Scheduling approach | Fixed historical average | Real-time dynamic update | More adaptive |

## Interpretation

The results show that real-time phase detection can convert surgical progress data into operational action. Instead of waiting until a surgery ends or relying on static estimates, the hospital can update the next scheduled case based on live intra-surgical information.

## Consulting-style implications

For a healthcare organization, this approach can support:

- Operating room utilization improvement
- Patient waiting-time reduction
- Better anesthesia and preparation coordination
- More reliable daily surgical schedules
- Improved patient experience
- More data-driven OR management

## Implementation considerations

For practical deployment, a hospital would need:

- Reliable video data access
- Clinical workflow validation
- Integration with scheduling systems
- Staff notification protocols
- Model monitoring and performance tracking
- Governance around clinical data privacy and decision support
