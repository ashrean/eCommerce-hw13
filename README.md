# eCommerce

# Table of Contents
- [eCommerce](#ecommerce)
- [Table of Contents](#table-of-contents)
- [Description](#description)
- [Installtion Instructions](#installtion-instructions)
- [Github Account](#github-account)
- [Images](#images)
- [Contacts](#contacts)
- [Code Snippets](#code-snippets)
- [Resources](#resources)


# Description
This project requires the developer to build the backend for an e-commerce site. The developer will use their knowledge of using Express, API, and Sequelize to interact with the MySQL database.

# Installtion Instructions
There is a few steps to do.
- In your terminal run `mysq -u root -p`
- Run `SOURCE ./db/schema.sql`
- Then in another terminal
- Run `npm run seed`
- Then we can run `npm start`

# Github Account
- [GitHub](https://github.com/ashrean)
- [Video Link](./images/Untitled_%20Feb%207%202023%2012_00%20AM.webm)

# Images
![alt text](./images/Screenshot%202023-02-06%20at%209.39.20%20PM.png)

# Contacts
- [Email](sese.ashrean@gmail.com)
- [Linkedin](https://www.linkedin.com/in/ashleyrean/)

# Code Snippets
```
router.get('/', async (req, res) => {
  try{
    const categoryData = await category.findAll({
      include: [{ model: Product}]
    });
    res.status(200).json(categoryData)
  } catch (err) {
    res.status(500).json(err);
  }
});
```

# Resources
- Class Activites/Mini Projects
- [Sequelize](https://www.npmjs.com/package/sequelize)
- [MySql](https://www.npmjs.com/package/mysql2)
- [Express](https://www.npmjs.com/package/express)
