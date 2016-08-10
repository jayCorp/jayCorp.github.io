---
layout: post
title: Heroku to Amazon
---

Elastic Beanstalk

OpWorks

[Comparing Heroku and Amazon PostreSQL](https://blog.codeship.com/heroku-postgresql-versus-amazon-rds-postgresql/)

[Comparing Hardware](http://stackoverflow.com/a/9803182)

You can figure out what kind of underlaying hardware your dynos are running on with `heroku run console`  


{% highlight ruby %}

free -ht
	             total       used       free     shared    buffers     cached
	Mem:           60G        54G       5.3G        41M       3.5G        15G
	-/+ buffers/cache:        35G        24G
	Swap:          60G       1.8G        59G
	Total:        121G        56G        64G

{% endhighlight %}



{% highlight ruby %}
cat /proc/cpuinfo


	processor	: 0
	vendor_id	: GenuineIntel
	cpu family	: 6
	model		: 62
	model name	: Intel(R) Xeon(R) CPU E5-2670 v2 @ 2.50GHz
	stepping	: 4
	microcode	: 0x428
	cpu MHz		: 2494.068
	cache size	: 25600 KB
	physical id	: 0
	siblings	: 8
	core id		: 0
	cpu cores	: 4
	apicid		: 0
	initial apicid	: 0
	fpu		: yes
	fpu_exception	: yes
	cpuid level	: 13
	wp		: yes
	flags		: fpu vme de pse tsc msr pae mce cx8 apic sep mtrr pge mca cmov pat pse36 clflush mmx fxsr sse sse2 ht syscall nx rdtscp lm constant_tsc rep_good nopl xtopology eagerfpu pni pclmulqdq ssse3 cx16 pcid sse4_1 sse4_2 x2apic popcnt tsc_deadline_timer aes xsave avx f16c rdrand hypervisor lahf_lm xsaveopt fsgsbase smep erms
	bogomips	: 4988.13
	clflush size	: 64
	cache_alignment	: 64
	address sizes	: 46 bits physical, 48 bits virtual
	power management:

...cont x8
{% endhighlight %}