一些个人意见，仅供参考：

1): 如果一个user login  之后，从目前的er 图中， 我们没办法知道该用户是一个doctor, patient or admin user. 当然，等回到作class diagram 的时候，或者就能知道了。
提出这个问题，就作为一个reminder 吧。

2): 如果直接作entity  的 class digram 如何？也就是直接从oo 去考虑，er 图直接由工具生成(如果有需要查看er 图的话）。

3): 目前role table, 有这样的description:
  * 001,0002,0004,0008: doctor CRUD
  * 010,0020,0040,0080: booking CRUD
  * 100,0200,0400,0800: consulting CRUD

好像这个不是用来作role 的功能：），到象是用来直接作acl 的?
对于一个role 表来说，一个用户可能属于多个role，也可能只有一个role。

象我们目前的系统里面，或许可以抽取出两个roles: patient 和 doctor (admin??)，这样用户login 之后，我们就知道该用户是user or patient.

4): 增加一个acl 表。当然也看我们目前是否有这个需要了。 比如是否需要控制用户的crud. acl 中可以体现下面信息，
> userid, resource type, canRead, canCreate, canUpdate, canDelete.

5): 建议增加一张service 表，用来表明某个医生能够提供的服务种类，服务时间阿 什么的。这样可以将doctor 里面的一些信息抽取出来放到这个service 表中去。