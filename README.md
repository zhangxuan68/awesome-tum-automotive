# Awesome TUM Automotive

慕尼黑工业大学(Technical University of Munich, TUM)与**汽车、自动驾驶、智慧出行**相关的开源项目汇总。

内容整理自 TUM 车辆技术研究所(FTM)与自动驾驶系统研究所(AVS)官方开源页面、CommonRoad 官方工具列表,以及各组织的 GitHub 主页。

---

## 目录

- [组织入口](#组织入口)
- [自动驾驶 · 规划与决策](#自动驾驶--规划与决策)
- [自动驾驶 · 感知与融合](#自动驾驶--感知与融合)
- [定位与建图](#定位与建图)
- [自动驾驶赛车](#自动驾驶赛车)
- [车辆动力学与控制](#车辆动力学与控制)
- [仿真与基准工具](#仿真与基准工具)
- [数据集](#数据集)
- [智慧出行与电动化](#智慧出行与电动化)
- [其他工具](#其他工具)

---

## 组织入口

| 组织 | 方向 | 链接 |
|---|---|---|
| **TUMFTM** | 车辆技术研究所(Lehrstuhl für Fahrzeugtechnik),体量最大 | https://github.com/TUMFTM |
| **TUM-AVS** | 自动驾驶系统研究所,规划与感知为主 | https://github.com/TUM-AVS |
| **CommonRoad** | 运动规划基准与工具链(TUM Cyber-Physical Systems) | https://github.com/CommonRoad |
| **TUMRT** | 赛车实时控制与三维规划 | https://github.com/TUMRT |
| **tum-traffic-dataset** | 路侧与 V2X 协同感知数据集 | https://github.com/tum-traffic-dataset |

---

## 自动驾驶 · 规划与决策

| 项目 | 说明 |
|---|---|
| [Frenetix-Motion-Planner](https://github.com/TUM-AVS/Frenetix-Motion-Planner) | 采样式 Frenet 轨迹规划框架,含 C++ 加速版,AVS 组的核心规划器 |
| [OcclusionAwareMotionPlanning](https://github.com/TUM-AVS/OcclusionAwareMotionPlanning) | 在 Frenetix 基础上加入遮挡与风险感知,面向视野受限的城市场景 |
| [PedestrianAwareMotionPlanning](https://github.com/TUM-AVS/PedestrianAwareMotionPlanning) | 带行人预测、风险评估与行为感知决策的轨迹规划 |
| [DualAD](https://github.com/TUM-AVS/DualAD) | 规则式运动规划与大语言模型推理结合,处理复杂驾驶场景 |
| [From-Words-to-Collisions](https://github.com/TUM-AVS/From-Words-to-Collisions) | 用 LLM 评估并对抗式生成安全关键驾驶场景 |
| [EthicalTrajectoryPlanning](https://github.com/TUMFTM/EthicalTrajectoryPlanning) | 把伦理风险分配纳入轨迹规划 |
| [GraphBasedLocalTrajectoryPlanner](https://github.com/TUMFTM/GraphBasedLocalTrajectoryPlanner) | 基于图搜索的局部轨迹规划 |
| [TrajectorySupervisor](https://github.com/TUMFTM/TrajectorySupervisor) | 规划轨迹的在线安全监控模块 |

---

## 自动驾驶 · 感知与融合

| 项目 | 说明 |
|---|---|
| [CameraRadarFusionNet](https://github.com/TUMFTM/CameraRadarFusionNet) | 相机 + 毫米波雷达融合检测网络,被引用较多的参考实现 |
| [RadarVoxelFusionNet](https://github.com/TUMFTM/RadarVoxelFusionNet) | 雷达体素融合的三维目标检测 |
| [RadarGNN](https://github.com/TUMFTM/RadarGNN) | 面向雷达点云的图神经网络 |
| [DPFT](https://github.com/TUMFTM/DPFT) | 雷达与相机融合的 Transformer 检测方法 |
| [CamRaDepth](https://github.com/TUM-AVS/CamRaDepth) | 融合图像、语义分割与稀疏雷达的单目深度估计 |
| [Multi_LiCa](https://github.com/TUMFTM/Multi_LiCa) | 多激光雷达自动外参标定 |
| [GMMCalib](https://github.com/TUMFTM/GMMCalib) | 基于高斯混合模型的标定方法 |
| [FusionTracking](https://github.com/TUMFTM/FusionTracking) | 多传感器目标融合跟踪 |
| [Snapshot](https://github.com/TUMFTM/Snapshot) | 轨迹预测方法 |

---

## 定位与建图

| 项目 | 说明 |
|---|---|
| [ORB_SLAM3_RGBL](https://github.com/TUM-AVS/ORB_SLAM3_RGBL) | 为 ORB-SLAM3 增加激光雷达深度模式 |
| [FlexMap_Fusion](https://github.com/TUM-AVS/FlexMap_Fusion) | 多激光雷达离线建图 + 在线定位,基于 KISS-ICP |
| [FlexCloud](https://github.com/TUMFTM/FlexCloud) | 定位相关的点云处理 |
| [OpenLiDARMap](https://github.com/TUMFTM/OpenLiDARMap) | 激光雷达地图与定位 |
| [orbslam-map-saving-extension](https://github.com/TUMFTM/orbslam-map-saving-extension) | ORB-SLAM 地图保存与复用扩展 |
| [3DVehicleDynamicsStateEstimation](https://github.com/TUM-AVS/3DVehicleDynamicsStateEstimation) | 三维点质量扩展卡尔曼滤波状态估计 |
| [Lane_Level_Matching](https://github.com/TUMFTM/Lane_Level_Matching) | 车道级地图匹配 |

---

## 自动驾驶赛车

源自 Roborace 与 Indy Autonomous Challenge 的技术积累,是 TUM 在自动驾驶领域最有辨识度的一块。

| 项目 | 说明 |
|---|---|
| [global_racetrajectory_optimization](https://github.com/TUMFTM/global_racetrajectory_optimization) | **全局最优赛车线生成**,这一组里使用最广的库 |
| [racetrack-database](https://github.com/TUMFTM/racetrack-database) | 赛道中心线与边界数据集 |
| [laptime-simulation](https://github.com/TUMFTM/laptime-simulation) | 圈速仿真 |
| [race-simulation](https://github.com/TUMFTM/race-simulation) | 比赛策略仿真(进站、轮胎管理等) |
| [online_3D_racing_line_planning](https://github.com/TUMRT/online_3D_racing_line_planning) | 考虑坡度与倾角的三维赛车线在线规划 |
| [sampling_based_3D_local_planning](https://github.com/TUMRT/sampling_based_3D_local_planning) | 三维局部采样规划 |
| [MixNet](https://github.com/TUMFTM/MixNet) | 赛车场景轨迹预测 |
| [RoboRacer-3DLiDAR](https://github.com/TUM-AVS/RoboRacer-3DLiDAR) | F1Tenth / RoboRacer 平台的三维激光 SLAM 与驱动 |

---

## 车辆动力学与控制

| 项目 | 说明 |
|---|---|
| [mod_vehicle_dynamics_control](https://github.com/TUMFTM/mod_vehicle_dynamics_control) | 完整的车辆动力学控制栈(Simulink 实现) |
| [Open-Car-Dynamics](https://github.com/TUMFTM/Open-Car-Dynamics) | 开源车辆动力学模型 |
| [sim_vehicle_dynamics](https://github.com/TUMFTM/sim_vehicle_dynamics) | 仿真用车辆动力学模型 |
| [Tire_Parameter_and_Uncertainty_Estimation](https://github.com/TUMFTM/Tire_Parameter_and_Uncertainty_Estimation) | 轮胎参数与不确定度辨识 |
| [TAM__long_acc_control](https://github.com/TUMFTM/TAM__long_acc_control) | 纵向加速度控制 |

---

## 仿真与基准工具

### CommonRoad 工具链

TUM Cyber-Physical Systems 组维护,运动规划领域应用广泛的基准平台。组织主页:https://github.com/CommonRoad

| 工具 | 说明 |
|---|---|
| CommonRoad Input-Output | 场景与规划问题的读写及可视化 |
| CommonRoad Scenario Designer | OpenStreetMap / OpenDRIVE 地图转换,配合 SUMO 的场景编辑 GUI |
| CommonRoad Drivability Checker | 轨迹可行性与碰撞检测,曲线坐标系变换 |
| CommonRoad Route Planner | 为运动规划器提供高层引导与参考路径 |
| CommonRoad-Search | 基于运动基元的有信息/无信息搜索算法 |
| CommonRoad-Reach | 动态交通中的可达集计算与行驶走廊提取 |
| CommonRoad-RL | 基于 Stable Baselines 的强化学习运动规划 |
| CommonRoad-Geometric | 把交通场景构建为 PyTorch 图数据集 |
| CommonRoad-CriMe | 危险度量的统一记号、车辆模型与坐标系 |
| CommonRoad-OpenSCENARIO-Converter | OpenSCENARIO 与 CommonRoad 场景互转 |

### 其他仿真工具

| 项目 | 说明 |
|---|---|
| [sumo-docker](https://github.com/TUMFTM/sumo-docker) | SUMO 交通仿真的容器化部署 |
| [edgar_digital_twin](https://github.com/TUM-AVS/edgar_digital_twin) | EDGAR 自动驾驶研究车的数字孪生,支持二维与三维仿真器 |
| [ros2_latency_analysis](https://github.com/TUM-AVS/ros2_latency_analysis) | 通过静态代码分析构建 ROS 2 C++ 系统数据流图,用于时延分析 |

---

## 数据集

| 项目 | 说明 |
|---|---|
| [tum-traffic-dataset-dev-kit](https://github.com/tum-traffic-dataset/tum-traffic-dataset-dev-kit) | TUMTraf / Providentia++ 路侧与 V2X 协同感知数据集开发包 |
| [truckscenes-devkit](https://github.com/TUMFTM/truckscenes-devkit) | MAN TruckScenes 卡车自动驾驶数据集开发包 |
| [ESP-Dataset](https://github.com/TUM-AVS/ESP-Dataset) | 紧急场景长时行为预测数据集,含语义环境信息 |
| [Sim2RealDistributionAlignedDataset](https://github.com/TUMFTM/Sim2RealDistributionAlignedDataset) | 仿真到真实分布对齐数据集 |
| [target-bench](https://github.com/TUM-AVS/target-bench) | 测试视频世界模型无图语义目标导航能力的基准 |
| [A2RL Vmax 自动驾驶赛车数据集](https://tum-avs.github.io/A2RL_Dataset_website/) | Yas Marina 赛道多车高速交互的激光雷达、雷达与车辆数据 |

---

## 智慧出行与电动化

| 项目 | 说明 |
|---|---|
| [UrbanEV](https://github.com/TUMFTM/UrbanEV) | 城市电动车分析 |
| [Hamburg-Public-Charging-Station-Utilization](https://github.com/TUMFTM/Hamburg-Public-Charging-Station-Utilization) | 汉堡公共充电桩使用率分析 |
| [transport-system-simulation](https://github.com/TUMFTM/transport-system-simulation) | 交通系统仿真 |
| [passenger-vehicle-clustering](https://github.com/TUMFTM/passenger-vehicle-clustering) | 乘用车聚类与可视化 |
| [european-bike-sharing-dataset](https://github.com/TUMFTM/european-bike-sharing-dataset) | 欧洲共享单车数据集 |
| [ExternalCostsBikes_public](https://github.com/TUMFTM/ExternalCostsBikes_public) | 自行车外部成本分析 |
| [GIS-Mobility-Toolkit](https://github.com/TUMFTM/GIS-Mobility-Toolkit) | 出行分析的 GIS 工具集 |
| [dt-cargo](https://github.com/TUMFTM/dt-cargo) | 货运相关工具 |
| [RID](https://github.com/TUMFTM/RID) | 屋顶信息数据集 |
| [pv-diagnostic-tool](https://github.com/TUMFTM/pv-diagnostic-tool) | 光伏诊断工具 |
| [SASIM](https://github.com/TUMFTM/SASIM) | 出行仿真相关 |
| [MAGIS](https://github.com/TUMFTM/MAGIS) | GIS 相关工具 |
| [sm-data-desk](https://github.com/TUMFTM/sm-data-desk) | 智慧出行数据工具 |
| [Labcourse-Mobility-Data-Analysis](https://github.com/TUMFTM/Labcourse-Mobility-Data-Analysis) | 出行数据分析实验课材料 |

---

## 其他工具

| 项目 | 说明 |
|---|---|
| [teleoperated_driving](https://github.com/TUMFTM/teleoperated_driving) | 远程遥控驾驶 |
| [uds-decoder](https://github.com/TUMFTM/uds-decoder) | UDS 诊断报文解码 |
| [TAM__common](https://github.com/TUMFTM/TAM__common) | TAM 软件栈公共代码 |
| [TAM__msgs](https://github.com/TUMFTM/TAM__msgs) | TAM 软件栈消息定义 |
| [tsl](https://github.com/TUMFTM/tsl) | TUMFTM 工具库 |

---

## 说明

- 项目清单来源于 TUM 官方开源页面与各 GitHub 组织主页。部分项目(尤其是智慧出行类)官方页面仅给出名称,描述为根据项目名与所属分类推断,使用前建议以仓库 README 为准。
- FTM 官方页面注明赛车方向"当前软件栈即将发布",后续可能有新增项目。
- 各项目许可证不尽相同,商用前请逐个确认。

## 参考来源

- [TUM FTM Open Source Software](https://www.mos.ed.tum.de/en/ftm/open-source-software/)
- [TUM AVS Software](https://www.mos.ed.tum.de/en/avs/software/)
- [CommonRoad 官方工具列表](https://ce.cit.tum.de/cps/software/commonroad)
