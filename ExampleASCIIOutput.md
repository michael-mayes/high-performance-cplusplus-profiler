
```
> Raw run time 5956.56 mcycles
> Total calls 9937241, per call overhead 75 cycles, rdtsc overhead 33 cycles, estimated overhead 745.71 mcycles

+- 76.95 mcycles, 1 calls, 76945653 cycles avg, 100.00%: /Main
 \+- 37.33 mcycles, 1 calls, 37325745 cycles avg, 48.51%: struct node_t *__cdecl create(struct node_t *,const int,int,struct v_t,struct v_t,double)
  | +- 37.31 mcycles, 9 calls, 4145976 cycles avg, 48.49%: struct node_t *__cdecl create(struct node_t *,const int,int,struct v_t,struct v_t,double)
  | | +- 37.27 mcycles, 81 calls, 460159 cycles avg, 48.44%: struct node_t *__cdecl create(struct node_t *,const int,int,struct v_t,struct v_t,double)
  | | | +- 36.92 mcycles, 729 calls, 50647 cycles avg, 47.98%: struct node_t *__cdecl create(struct node_t *,const int,int,struct v_t,struct v_t,double)
  | | | | +- 33.83 mcycles, 6561 calls, 5156 cycles avg, 43.97%: struct node_t *__cdecl create(struct node_t *,const int,int,struct v_t,struct v_t,double)
  | | | | | -- 5.73 mcycles, 59049 calls, 97 cycles avg, 7.45%: struct node_t *__cdecl create(struct node_t *,const int,int,struct v_t,struct v_t,double)
  | | | |  \-- 1.89 mcycles, 6561 calls, 288 cycles avg, 2.46%: __thiscall basis_t::basis_t(const struct v_t &)
  | | |  \-- 0.17 mcycles, 729 calls, 240 cycles avg, 0.23%: __thiscall basis_t::basis_t(const struct v_t &)
  | |  \-- 0.02 mcycles, 81 calls, 221 cycles avg, 0.02%: __thiscall basis_t::basis_t(const struct v_t &)
  |  \-- 0.00 mcycles, 9 calls, 220 cycles avg, 0.00%: __thiscall basis_t::basis_t(const struct v_t &)
   \-- 0.00 mcycles, 1 calls, 585 cycles avg, 0.00%: __thiscall basis_t::basis_t(const struct v_t &)


+- 11629.56 mcycles, 32 calls, 363423883 cycles avg, 100.00%: unsigned long __stdcall trace_launcher(void *)
 \+- 11089.25 mcycles, 4194304 calls, 2644 cycles avg, 95.35%: double __cdecl ray_trace(const struct node_t *const ,const struct ray_t &)
  | -- 7044.50 mcycles, 4194304 calls, 1680 cycles avg, 60.57%: void __cdecl node_t::intersect<false>(const struct ray_t &,struct hit_t &)
   \-- 3390.46 mcycles, 1474822 calls, 2299 cycles avg, 29.15%: void __cdecl node_t::intersect<true>(const struct ray_t &,struct hit_t &)



top 7 functions (self time)
> 7044.50 mcycles, 4194304 calls, 1680 cycles avg, 60.18%: void __cdecl node_t::intersect<false>(const struct ray_t &,struct hit_t &)
> 3390.46 mcycles, 1474822 calls, 2299 cycles avg, 28.96%: void __cdecl node_t::intersect<true>(const struct ray_t &,struct hit_t &)
> 654.29 mcycles, 4194304 calls, 156 cycles avg, 5.59%: double __cdecl ray_trace(const struct node_t *const ,const struct ray_t &)
> 540.31 mcycles, 32 calls, 16884811 cycles avg, 4.62%: unsigned long __stdcall trace_launcher(void *)
> 39.62 mcycles, 1 calls, 39619908 cycles avg, 0.34%: /Main
> 35.24 mcycles, 66430 calls, 530 cycles avg, 0.30%: struct node_t *__cdecl create(struct node_t *,const int,int,struct v_t,struct v_t,double)
> 2.08 mcycles, 7381 calls, 282 cycles avg, 0.02%: __thiscall basis_t::basis_t(const struct v_t &)
```