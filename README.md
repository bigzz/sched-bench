Storage-I/O Scheduler Benchmark. 
A bash script to measure disk performance under 
different available schedulers such as DEADLINE, CFQ, NOOP, BFQ

The benchmark script uses bonnie++, dd and hdparm to 
measure performance using each available io scheduler.

Benchmarks can take a long time depenend on your ram size.
Make sure you have at least 2x ramsize free as diskspace

To change your io scheduler permanently edit 
/etc/default/grub add elevator= to GRUB_CMDLINE_LINUX
and update-grub (grub.cfg)

