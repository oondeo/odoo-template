# BUILD
Must add a Dockerfile in odoo directory to use custom functions.

# ENV
        - args:
            - '--dev'
            - all
          env:
            - name: PGHOST
              value: postgresql.oondeo
            - name: PGUSER
              value: agrifercan
            - name: PGPASSWORD
              value: db2019_
            - name: PGDATABASE
              value: agrifercan.sol.oondeo.es
            - name: PROXY_MODE
              value: 'true'
            - name: DB_FILTER
              value: agrifercan.sol.oondeo.es
          image: 'agrifercan:latest'
