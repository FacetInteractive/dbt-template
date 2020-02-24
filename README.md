# dbt Project Setup

Please fork this template and perform the initial setup steps:

1. [ ] Find and replace `<clientcode>` with the appropriate shortname for the analytics project.
2. [ ] Copy the `.env.dist` to `.env` and fill in the information.
3. [ ] Review the `packages.yml` and make sure they apply for this project. 
4. [ ] Review `dbt_project.yml`

## Developing with Lando

1. Download the [latest version of Lando](https://github.com/lando/lando/releases).
2. If you already have Docker installed, you may need to uninstall it in order to get the correct version for Lando. 
3. Run `lando start`.
4. SSH into Python environment with `lando ssh`, where you can run `dbt <command>` directly.
5. Alternatively review the `lando dbt` command if you don't want to SSH into the container. It will accept commands in the form of `lando dbt <command>`.

# dbt Starter Project

### Using the starter project

Try running the following commands:
- dbt deps
- dbt run
- dbt test


### Resources:
- Learn more about dbt [in the docs](https://docs.getdbt.com/docs/overview)
- Check out [Discourse](https://discourse.getdbt.com/) for commonly asked questions and answers
- Join the [chat](http://slack.getdbt.com/) on Slack for live discussions and support
- Find [dbt events](https://events.getdbt.com) near you
- Check out [the blog](https://blog.getdbt.com/) for the latest news on dbt's development and best practices


### Template To Do

- [ ] Mount a separate Python environment for Singer
- [ ] Implement a `singer-db-import` Lando command to pipe in SQL data to the mounted PgSQL database
- [ ] Provide instructions for `pgsql` import with Lando 