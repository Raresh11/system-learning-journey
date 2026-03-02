# Title: System Risks – Basic Web Architecture

## 1. Single Point of Failure – Database

**Risk**
If the database is unavailable, the entire system becomes unavailable.

**Impact**
Full downtime
Revenue loss
Incident severity: High

**Mitigation** (conceptual)
Primary + replica database
Automated backups
Health checks and failover strategy

## 2. Single Backend Instance

**Risk**
If the only backend server crashes, no requests can be processed.

**Impact**
Service unavailable
Poor user experience

**Mitigation**
Multiple backend instances
Load balancer

## 3. Slow Database Queries

**Risk**
High latency due to inefficient queries.

**Impact**
Slow response time
Timeouts under load

**Mitigation**
Query optimization
Caching layer (future improvement)

## 4. No Monitoring

**Risk**
Failures are detected only after users complain.

**Impact**
Longer incident resolution time

**Mitigation**
Basic monitoring and alerting
