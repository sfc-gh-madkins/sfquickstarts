author: miles.adkins@snowflake.com
id: hex
summary: This lab will walk you through how to use Snowflake and Hex.
categories: Getting Started
environments: web
status: Published
feedback link: https://github.com/Snowflake-Labs/sfguides/issues
tags: Hex, Notebooks, Partner Connect

# {title} with Snowflake and Hex

<!-- ------------------------ -->
## Lab Overview
Duration: 5

{use case / lab overview}

### Prerequisites
- {list}

### What You'll Learn
- {list}
- Use Snowflake’s “Partner Connect” to seamlessly create a Hex trial

### What You’ll Need
- A [Snowflake](https://signup.snowflake.com/) Account (if you are using an enterprise account through your organization, it is unlikely that you will have the privileges to use the `ACCOUNTADMIN` role, which is required for this lab).

### What You’ll Build
- {list}

<!-- ------------------------ -->
## Setting up Snowflake
Duration: 5

The first thing you will need to do is download the following .sql file that contains a series of SQL commands we will execute throughout this lab.

<button>
  [Download .sql File]({url to sql})
</button>
<br/><br/>

At this point, log into your Snowflake account and open a new `Worksheet`. If you have just created a free trial account, you will land in the `Learn` section. Simply navigate to the `Worksheets` tab on the left and click `+ Worksheet` in the top right hand corner.

![](assets/p51.png)
<br/><br/>

To ingest our script in the Snowflake UI, click the down arrow next to the time your notebook was created in the top left hand side of your screen and load our `Snowflake_Hex_VHOL_guies.sql` script using the `Import SQL from File` button. You can also change the name of this worksheet to "Snowflake-Hex VHOL"

![](assets/p53.png)
<br/><br/>

Snowflake provides "worksheets" as the spot for you to execute your code. For each worksheet you create, you will need to set the “context” so the worksheet knows how to behave. A “context” in Snowflake is made up of 4 distinctions that must be set before we can perform any work: the “role” we want to act as, the “database” and “schema” we want to work with, and the “warehouse” we want to perform the work.

Lets go ahead and set the role we want to act as, which will be `ACCOUNTADMIN` to begin with. This can either be done manually in the UI or programmatically in a worksheet (`ACCOUNTADMIN` is the default role for a first time user). Lets do so programmatically in our worksheet by executing our first line of code:

```sql
USE ROLE accountadmin;
```

To execute this code, all we need to do is place our cursor on the line we wish to run and then either hit the "run" button at the top left of the worksheet or press `Cmd/Ctrl + Enter`.

 In addition to traditional SQL statements, Snowflake Data Definition ([DDL](https://docs.snowflake.com/en/sql-reference/sql-ddl-summary.html)) commands, such as setting the worksheet context, can also be written and executed within the worksheet.

Each step throughout the guide has an associated SQL command to perform the work we are looking to execute, and so feel free to step through each action running the code line by line as we walk through the lab.

<!-- ------------------------ -->
## Connecting Snowflake with Hex
Duration: 10

At this point in time, we have our data sitting in an optimized table within Snowflake that is available for a variety of different downstream functions. Snowflake does not offer notebook capabilities, and therefore, happily partners with the leading cloud notebook  partners in the industry.

Snowflake's Partner Connect feature allows you to seamlessly get started with partner tools and manages most of the connection details for you to get up and running as quickly as possible. To get here, click our "Home" button and then navigate to "Admin" and then "Partner Connect". This should take you to the following screen where you will see many of the Snowflake partners, and through a simple method of setting up an account and integration, allow you to quickly move data into a partner tool. Click the "Data Science & ML" category and click "Hex".

![](assets/p62.png)
<br/><br/>

We have all the Snowflake objects we need created already, so press "Connect".

![](assets/p65.png)

<!-- ------------------------ -->
## Getting Started with Hex
Duration: 10

Go to your email, and verify your account, you will be redirected to the Hex account registration page. ...

<!-- ------------------------ -->
