FH-RBAC
=======

由于每次开发新项目都需要一个权限管理系统，为了解决重复开发让成本增加的问题，特此开发一套通用权限管理系统，方便大家在此基础上开发出更多更优秀的软件产品。这不是一个权限管理系统，而是一个项目开发的开始，更是一个成功的学习案例。  RBAC认为权限授权实际上是Who、What、How的问题。在RBAC模型中，who、what、how构成了访问权限三元组,也就是“Who对What(Which)进行How的操作”。           Who：权限的拥用者或主体（如Principal、User、Group、Role、Actor等等）  What：权限针对的对象或资源（Resource、Class）。           How：具体的权限（Privilege,正向授权与负向授权）。           Operator：操作。表明对What的How操作。也就是Privilege+Resource         Role：角色，一定数量的权限的集合。权限分配的单位与载体,目的是隔离User与Privilege的逻辑关系.           Group：用户组，权限分配的单位与载体。权限不考虑分配给特定的用户而给组。组可以包括组(以实现权限的继承)，也可以包含用户，组内用户继承 组的权限。User与Group是多对多的关系。Group可以层次化，以满足不同层级权限控制的要求。         RBAC的关注点在于Role和User, Permission的关系。称为User assignment(UA)和Permission assignment(PA).关系的左右两边都是Many-to-Many关系。就是user可以有多个role，role可以包括多个user。
