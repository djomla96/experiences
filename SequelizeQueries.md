 
# DISTINCT WITH INCLUDES
```js
await ContactLog.findAll({
    where: {
        message: {
            [Op.iLike]: '%165531%'
        }
    },
    attributes: [Sequelize.literal('DISTINCT ON("UserId") 1'), '*'],
    include: [{model: User, as: "User"}],
    raw: true -!!!!!!!
})
```
