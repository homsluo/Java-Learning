# 2020/7/29
+ 往已经存有数据的db里存数据会报错，需要设置默认值，可以在上面加@Column(columnDefinition = "int8 default 0")
+ 改变JPARpository里默认的IDtype <T,ID(String, Long, UUID...)> 即可适用于所有JPARpository自带method
+ JPARepository默认方法可以有findxxByxx, 还有existsxxByxx返回boolean可用于验证
