---
{
    "title": "调优概述",
    "language": "zh-CN"
}
---

<!-- 
Licensed to the Apache Software Foundation (ASF) under one
or more contributor license agreements.  See the NOTICE file
distributed with this work for additional information
regarding copyright ownership.  The ASF licenses this file
to you under the Apache License, Version 2.0 (the
"License"); you may not use this file except in compliance
with the License.  You may obtain a copy of the License at

  http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing,
software distributed under the License is distributed on an
"AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
KIND, either express or implied.  See the License for the
specific language governing permissions and limitations
under the License.
-->

查询性能调优是一个系统工程，需要从多层次、多维度对数据库系统进行调优。以下是调优流程和方法论概述：

1. 首先，业务人员和数据库管理员（DBA）需要对所使用的数据库系统有全面的了解，包括业务系统使用的硬件、集群的规模、使用的数据库软件版本，以及具体软件版本所提供的特性等。
2. 其次，一个好用的性能诊断工具是定位性能问题的必要前提。只有高效快速地定位到问题 SQL 或者慢 SQL，才能进行后续的具体性能调优流程。
3. 在进入性能调优环节之后，一些常用的性能分析工具是必不可少的。这其中包括当前运行数据库系统自带的特有工具，以及操作系统层面的通用工具。
4. 有了上述工具之后，使用特有工具可以获取 SQL 运行在当前数据库系统上的详细信息，帮助定位性能瓶颈，同时，通用工具也可以作为辅助分析手段帮助定位问题。

综上所述，性能调优需要从全局视角来评估当前系统的性能状况。首先需要定位存在性能问题的业务 SQL，然后运用分析工具发现性能瓶颈，最后实施具体的调优操作。

基于上述调优流程和方法论，Apache Doris 在上述各个层面都提供了相应的工具。下文将分别对性能[诊断工具](diagnostic-tools.md)、[分析工具](analysis-tools.md)、[调优流程](tuning-process.md)三个方面进行介绍。