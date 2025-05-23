# my-first-project
<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>环境感知与建模研究组</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://cdn.jsdelivr.net/npm/font-awesome@4.7.0/css/font-awesome.min.css" rel="stylesheet">
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        primary: '#165DFF',
                        secondary: '#36CFC9',
                        neutral: {
                            100: '#F5F7FA',
                            200: '#E4E7ED',
                            300: '#DCDFE6',
                            400: '#C0C4CC',
                            500: '#909399',
                            600: '#606266',
                            700: '#303133',
                            800: '#1E1E1E',
                        }
                    },
                    fontFamily: {
                        inter: ['Inter', 'sans-serif'],
                    },
                }
            }
        }
    </script>
    <style type="text/tailwindcss">
        @layer utilities {
            .content-auto {
                content-visibility: auto;
            }
            .card-hover {
                transition: all 0.3s ease;
            }
            .card-hover:hover {
                transform: translateY(-5px);
                box-shadow: 0 10px 25px -5px rgba(0, 0, 0, 0.1);
            }
        }
    </style>
</head>
<body class="font-inter bg-neutral-100 text-neutral-700">
    <!-- 导航栏 -->
    <nav class="bg-white shadow-md sticky top-0 z-50">
        <div class="container mx-auto px-4">
            <div class="flex justify-between items-center py-4">
                <div class="flex items-center">
                    <div class="w-10 h-10 rounded-full bg-primary flex items-center justify-center text-white mr-3">
                        <i class="fa fa-flask"></i>
                    </div>
                    <span class="text-xl font-bold text-primary">环境感知与建模研究组</span>
                </div>
                
                <!-- 桌面导航 -->
                <div class="hidden md:flex space-x-8">
                    <a href="#home" class="text-neutral-700 hover:text-primary font-medium transition-colors">首页</a>
                    <a href="#research" class="text-neutral-700 hover:text-primary font-medium transition-colors">研究方向</a>
                    <a href="#members" class="text-neutral-700 hover:text-primary font-medium transition-colors">研究团队</a>
                    <a href="#publications" class="text-neutral-700 hover:text-primary font-medium transition-colors">学术成果</a>
                    <a href="#facilities" class="text-neutral-700 hover:text-primary font-medium transition-colors">科研环境</a>
                    <a href="#contact" class="text-neutral-700 hover:text-primary font-medium transition-colors">联系我们</a>
                </div>
                
                <!-- 移动端菜单按钮 -->
                <button id="menu-toggle" class="md:hidden text-neutral-700 focus:outline-none">
                    <i class="fa fa-bars text-xl"></i>
                </button>
            </div>
        </div>
        
        <!-- 移动端菜单 -->
        <div id="mobile-menu" class="hidden md:hidden bg-white border-t">
            <div class="container mx-auto px-4 py-3 space-y-3">
                <a href="#home" class="block text-neutral-700 hover:text-primary font-medium transition-colors">首页</a>
                <a href="#research" class="block text-neutral-700 hover:text-primary font-medium transition-colors">研究方向</a>
                <a href="#members" class="block text-neutral-700 hover:text-primary font-medium transition-colors">研究团队</a>
                <a href="#publications" class="block text-neutral-700 hover:text-primary font-medium transition-colors">学术成果</a>
                <a href="#facilities" class="block text-neutral-700 hover:text-primary font-medium transition-colors">科研环境</a>
                <a href="#contact" class="block text-neutral-700 hover:text-primary font-medium transition-colors">联系我们</a>
            </div>
        </div>
    </nav>

    <!-- 首页/英雄区域 -->
    <section id="home" class="bg-gradient-to-r from-primary to-secondary text-white py-20 md:py-32">
        <div class="container mx-auto px-4 text-center">
            <h1 class="text-[clamp(2rem,5vw,3.5rem)] font-bold mb-6">环境感知与建模研究组</h1>
            <p class="text-[clamp(1rem,2vw,1.25rem)] mb-10 max-w-3xl mx-auto">
                致力于环境传感器网络、大气污染建模、水环境监测与生态环境遥感等领域的前沿研究
            </p>
            <div class="flex flex-wrap justify-center gap-4">
                <a href="#research" class="px-6 py-3 bg-white text-primary font-medium rounded-lg hover:bg-neutral-100 transition-colors">
                    了解研究方向
                </a>
                <a href="#contact" class="px-6 py-3 bg-transparent border-2 border-white text-white font-medium rounded-lg hover:bg-white/10 transition-colors">
                    联系我们
                </a>
            </div>
        </div>
    </section>

    <!-- 关于我们 -->
    <section class="py-16 bg-white">
        <div class="container mx-auto px-4">
            <div class="text-center mb-12">
                <h2 class="text-3xl font-bold text-neutral-800 mb-4">关于我们</h2>
                <div class="w-20 h-1 bg-primary mx-auto"></div>
            </div>
            
            <div class="max-w-3xl mx-auto">
                <p class="text-neutral-700 mb-6 text-center">
                    环境感知与建模研究组成立于2010年，致力于环境传感器网络、大气污染建模、水环境监测与生态环境遥感等领域的前沿研究。
                </p>
                <p class="text-neutral-700 mb-6 text-center">
                    研究组现有教授2名，副教授3名，讲师2名，研究生30余名。近年来，在Environmental Science & Technology、Water Research等期刊发表论文100余篇，主持国家重点研发计划、国家自然科学基金等项目20余项。
                </p>
            </div>
            
            <div class="grid grid-cols-2 md:grid-cols-4 gap-6 mt-12">
                <div class="bg-neutral-100 p-6 rounded-lg text-center">
                    <div class="text-4xl font-bold text-primary mb-2">50+</div>
                    <div class="text-neutral-600">研究项目</div>
                </div>
                <div class="bg-neutral-100 p-6 rounded-lg text-center">
                    <div class="text-4xl font-bold text-primary mb-2">100+</div>
                    <div class="text-neutral-600">学术论文</div>
                </div>
                <div class="bg-neutral-100 p-6 rounded-lg text-center">
                    <div class="text-4xl font-bold text-primary mb-2">30+</div>
                    <div class="text-neutral-600">研究生</div>
                </div>
                <div class="bg-neutral-100 p-6 rounded-lg text-center">
                    <div class="text-4xl font-bold text-primary mb-2">10+</div>
                    <div class="text-neutral-600">合作机构</div>
                </div>
            </div>
        </div>
    </section>

    <!-- 研究方向 -->
    <section id="research" class="py-16 bg-neutral-100">
        <div class="container mx-auto px-4">
            <div class="text-center mb-12">
                <h2 class="text-3xl font-bold text-neutral-800 mb-4">研究方向</h2>
                <div class="w-20 h-1 bg-primary mx-auto"></div>
            </div>
            
            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                <div class="bg-white rounded-lg shadow-md p-6 card-hover">
                    <div class="w-14 h-14 rounded-full bg-primary/10 flex items-center justify-center text-primary mb-4">
                        <i class="fa fa-cloud text-2xl"></i>
                    </div>
                    <h3 class="text-xl font-bold text-neutral-800 mb-3">大气环境监测与建模</h3>
                    <p class="text-neutral-600">
                        开发新型大气污染物监测技术，构建空气质量预测模型，研究大气污染传输与扩散规律。
                    </p>
                </div>
                
                <div class="bg-white rounded-lg shadow-md p-6 card-hover">
                    <div class="w-14 h-14 rounded-full bg-primary/10 flex items-center justify-center text-primary mb-4">
                        <i class="fa fa-tint text-2xl"></i>
                    </div>
                    <h3 class="text-xl font-bold text-neutral-800 mb-3">水环境监测与模拟</h3>
                    <p class="text-neutral-600">
                        研究流域水环境演化规律，开发水质模型与生态风险评估方法，支撑水资源保护与管理。
                    </p>
                </div>
                
                <div class="bg-white rounded-lg shadow-md p-6 card-hover">
                    <div class="w-14 h-14 rounded-full bg-primary/10 flex items-center justify-center text-primary mb-4">
                        <i class="fa fa-tree text-2xl"></i>
                    </div>
                    <h3 class="text-xl font-bold text-neutral-800 mb-3">生态环境遥感监测</h3>
                    <p class="text-neutral-600">
                        利用卫星遥感与无人机技术，开展区域生态环境监测与评估，为生态保护与修复提供技术支持。
                    </p>
                </div>
                
                <div class="bg-white rounded-lg shadow-md p-6 card-hover">
                    <div class="w-14 h-14 rounded-full bg-primary/10 flex items-center justify-center text-primary mb-4">
                        <i class="fa fa-microchip text-2xl"></i>
                    </div>
                    <h3 class="text-xl font-bold text-neutral-800 mb-3">环境传感器网络</h3>
                    <p class="text-neutral-600">
                        研究新型环境传感器技术、传感器网络优化部署与数据采集方法，实现对环境要素的实时监测。
                    </p>
                </div>
                
                <div class="bg-white rounded-lg shadow-md p-6 card-hover">
                    <div class="w-14 h-14 rounded-full bg-primary/10 flex items-center justify-center text-primary mb-4">
                        <i class="fa fa-database text-2xl"></i>
                    </div>
                    <h3 class="text-xl font-bold text-neutral-800 mb-3">环境大数据分析</h3>
                    <p class="text-neutral-600">
                        发展环境大数据处理、分析与挖掘技术，结合机器学习方法，揭示环境演变规律与驱动机制。
                    </p>
                </div>
                
                <div class="bg-white rounded-lg shadow-md p-6 card-hover">
                    <div class="w-14 h-14 rounded-full bg-primary/10 flex items-center justify-center text-primary mb-4">
                        <i class="fa fa-line-chart text-2xl"></i>
                    </div>
                    <h3 class="text-xl font-bold text-neutral-800 mb-3">环境决策支持系统</h3>
                    <p class="text-neutral-600">
                        集成环境模型、优化算法与决策理论，开发环境管理与决策支持系统，为环境政策制定提供科学依据。
                    </p>
                </div>
            </div>
        </div>
    </section>

    <!-- 研究团队 -->
    <section id="members" class="py-16 bg-white">
        <div class="container mx-auto px-4">
            <div class="text-center mb-12">
                <h2 class="text-3xl font-bold text-neutral-800 mb-4">研究团队</h2>
                <div class="w-20 h-1 bg-primary mx-auto"></div>
            </div>
            
            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                <div class="bg-white rounded-lg shadow-md overflow-hidden card-hover">
                    <img src="https://picsum.photos/id/1005/400/300" alt="张教授" class="w-full h-64 object-cover">
                    <div class="p-6">
                        <h3 class="text-xl font-bold text-neutral-800 mb-1">张教授</h3>
                        <p class="text-primary mb-3">实验室主任</p>
                        <p class="text-neutral-600 mb-4">
                            主要研究方向为大气环境监测与建模，主持国家重点研发计划项目2项，发表论文50余篇。
                        </p>
                        <div class="flex space-x-3">
                            <a href="#" class="text-neutral-600 hover:text-primary transition-colors">
                                <i class="fa fa-google"></i>
                            </a>
                            <a href="#" class="text-neutral-600 hover:text-primary transition-colors">
                                <i class="fa fa-researchgate"></i>
                            </a>
                            <a href="#" class="text-neutral-600 hover:text-primary transition-colors">
                                <i class="fa fa-linkedin"></i>
                            </a>
                        </div>
                    </div>
                </div>
                
                <div class="bg-white rounded-lg shadow-md overflow-hidden card-hover">
                    <img src="https://picsum.photos/id/1001/400/300" alt="李副教授" class="w-full h-64 object-cover">
                    <div class="p-6">
                        <h3 class="text-xl font-bold text-neutral-800 mb-1">李副教授</h3>
                        <p class="text-primary mb-3">水环境研究组组长</p>
                        <p class="text-neutral-600 mb-4">
                            主要研究方向为水环境监测与模拟，主持国家自然科学基金项目3项，发表论文30余篇。
                        </p>
                        <div class="flex space-x-3">
                            <a href="#" class="text-neutral-600 hover:text-primary transition-colors">
                                <i class="fa fa-google"></i>
                            </a>
                            <a href="#" class="text-neutral-600 hover:text-primary transition-colors">
                                <i class="fa fa-researchgate"></i>
                            </a>
                        </div>
                    </div>
                </div>
                
                <div class="bg-white rounded-lg shadow-md overflow-hidden card-hover">
                    <img src="https://picsum.photos/id/1000/400/300" alt="王讲师" class="w-full h-64 object-cover">
                    <div class="p-6">
                        <h3 class="text-xl font-bold text-neutral-800 mb-1">王讲师</h3>
                        <p class="text-primary mb-3">环境传感器网络研究组组长</p>
                        <p class="text-neutral-600 mb-4">
                            主要研究方向为环境传感器网络，主持国家自然科学基金青年基金1项，发表论文20余篇。
                        </p>
                        <div class="flex space-x-3">
                            <a href="#" class="text-neutral-600 hover:text-primary transition-colors">
                                <i class="fa fa-google"></i>
                            </a>
                            <a href="#" class="text-neutral-600 hover:text-primary transition-colors">
                                <i class="fa fa-github"></i>
                            </a>
                        </div>
                    </div>
                </div>
            </div>
            
            <div class="text-center mt-10">
                <a href="#" class="text-primary font-medium hover:underline">查看全部团队成员</a>
            </div>
        </div>
    </section>

    <!-- 学术成果 -->
    <section id="publications" class="py-16 bg-neutral-100">
        <div class="container mx-auto px-4">
            <div class="text-center mb-12">
                <h2 class="text-3xl font-bold text-neutral-800 mb-4">学术成果</h2>
                <div class="w-20 h-1 bg-primary mx-auto"></div>
            </div>
            
            <div class="bg-white rounded-lg shadow-md p-6 mb-8">
                <h3 class="text-xl font-bold text-neutral-800 mb-4">代表性论文</h3>
                
                <div class="space-y-4">
                    <div class="p-4 border-l-4 border-primary bg-neutral-50">
                        <p class="font-medium">Zhang, J., Li, Y., Wang, H., & Chen, X. (2023). A novel air quality prediction model based on hybrid deep learning approach. Environmental Science & Technology, 57(12), 4890-4901.</p>
                    </div>
                    
                    <div class="p-4 border-l-4 border-primary bg-neutral-50">
                        <p class="font-medium">Li, Y., Zhang, J., & Zhao, L. (2023). Optimized deployment of wireless sensor networks for urban air quality monitoring. Sensors and Actuators B: Chemical, 371, 132534.</p>
                    </div>
                    
                    <div class="p-4 border-l-4 border-primary bg-neutral-50">
                        <p class="font-medium">Wang, H., Zhang, J., & Chen, X. (2022). Integrated water quality assessment and prediction using machine learning techniques: A case study of Taihu Lake. Journal of Environmental Management, 318, 115412.</p>
                    </div>
                </div>
                
                <div class="text-right mt-6">
                    <a href="#" class="text-primary font-medium hover:underline">查看全部论文</a>
                </div>
            </div>
            
            <div class="bg-white rounded-lg shadow-md p-6">
                <h3 class="text-xl font-bold text-neutral-800 mb-4">科研项目</h3>
                
                <div class="space-y-4">
                    <div class="flex items-start">
                        <div class="w-10 h-10 rounded-full bg-primary/10 flex items-center justify-center text-primary mr-4 flex-shrink-0">
                            <i class="fa fa-flask"></i>
                        </div>
                        <div>
                            <h4 class="font-bold text-neutral-800 mb-1">国家重点研发计划项目：城市大气复合污染立体监测技术与设备研发</h4>
                            <p class="text-neutral-600">项目负责人：张教授</p>
                            <p class="text-sm text-neutral-500">2022-2026, 经费: 2000万元</p>
                        </div>
                    </div>
                    
                    <div class="flex items-start">
                        <div class="w-10 h-10 rounded-full bg-primary/10 flex items-center justify-center text-primary mr-4 flex-shrink-0">
                            <i class="fa fa-flask"></i>
                        </div>
                        <div>
                            <h4 class="font-bold text-neutral-800 mb-1">国家自然科学基金面上项目：基于多源数据融合的区域空气质量预测理论与方法研究</h4>
                            <p class="text-neutral-600">项目负责人：李副教授</p>
                            <p class="text-sm text-neutral-500">2023-2026, 经费: 65万元</p>
                        </div>
                    </div>
                    
                    <div class="flex items-start">
                        <div class="w-10 h-10 rounded-full bg-primary/10 flex items-center justify-center text-primary mr-4 flex-shrink-0">
                            <i class="fa fa-flask"></i>
                        </div>
                        <div>
                            <h4 class="font-bold text-neutral-800 mb-1">国家自然科学基金青年基金：基于无人机遥感的湖泊富营养化监测与预警研究</h4>
                            <p class="text-neutral-600">项目负责人：王讲师</p>
                            <p class="text-sm text-neutral-500">2021-2024, 经费: 28万元</p>
                        </div>
                    </div>
                </div>
                
                <div class="text-right mt-6">
                    <a href="#" class="text-primary font-medium hover:underline">查看全部项目</a>
                </div>
            </div>
        </div>
    </section>

    <!-- 科研环境 -->
    <section id="facilities" class="py-16 bg-white">
        <div class="container mx-auto px-4">
            <div class="text-center mb-12">
                <h2 class="text-3xl font-bold text-neutral-800 mb-4">科研环境</h2>
                <div class="w-20 h-1 bg-primary mx-auto"></div>
            </div>
            
            <div class="grid md:grid-cols-2 gap-8">
                <div>
                    <h3 class="text-xl font-bold text-neutral-800 mb-4">室内试验环境</h3>
                    <p class="text-neutral-600 mb-6">
                        实验室拥有环境模拟舱、空气质量监测设备、水质分析仪器、传感器研发平台等先进设备，可开展环境感知技术研发、环境过程模拟与分析等研究。
                    </p>
                    
                    <div class="grid grid-cols-2 gap-4">
                        <img src="https://picsum.photos/id/1069/400/300" alt="环境模拟舱" class="rounded-lg shadow-md">
                        <img src="https://picsum.photos/id/180/400/300" alt="空气质量监测设备" class="rounded-lg shadow-md">
                        <img src="https://picsum.photos/id/237/400/300" alt="水质分析仪器" class="rounded-lg shadow-md">
                        <img src="https://picsum.photos/id/1060/400/300" alt="传感器研发平台" class="rounded-lg shadow-md">
                    </div>
                </div>
                
                <div>
                    <h3 class="text-xl font-bold text-neutral-800 mb-4">野外试验环境</h3>
                    <p class="text-neutral-600 mb-6">
                        实验室在城市、郊区和农村地区建立了多个野外监测站点，配备了先进的监测设备，可开展长期环境观测与研究。
                    </p>
                    
                    <div class="grid grid-cols-2 gap-4">
                        <img src="https://picsum.photos/id/1058/400/300" alt="城市监测站点" class="rounded-lg shadow-md">
                        <img src="https://picsum.photos/id/1062/400/300" alt="农村监测站点" class="rounded-lg shadow-md">
                        <img src="https://picsum.photos/id/1063/400/300" alt="无人机监测系统" class="rounded-lg shadow-md">
                        <img src="https://picsum.photos/id/1067/400/300" alt="湖泊监测浮标" class="rounded-lg shadow-md">
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- 联系我们 -->
    <section id="contact" class="py-16 bg-neutral-100">
        <div class="container mx-auto px-4">
            <div class="text-center mb-12">
                <h2 class="text-3xl font-bold text-neutral-800 mb-4">联系我们</h2>
                <div class="w-20 h-1 bg-primary mx-auto"></div>
            </div>
            
            <div class="bg-white rounded-lg shadow-md p-8 max-w-3xl mx-auto">
                <div class="grid md:grid-cols-2 gap-8">
                    <div>
                        <h3 class="text-xl font-bold text-neutral-800 mb-4">联系方式</h3>
                        
                        <div class="space-y-4">
                            <div class="flex items-start">
                                <div class="w-10 h-10 rounded-full bg-primary/10 flex items-center justify-center text-primary mr-4">
                                    <i class="fa fa-map-marker"></i>
                                </div>
                                <div>
                                    <h4 class="font-bold text-neutral-800 mb-1">地址</h4>
                                    <p class="text-neutral-600">中国上海市浦东新区张江高科技园区XX大道123号XX大学环境学院</p>
                                </div>
                            </div>
                            
                            <div class="flex items-start">
                                <div class="w-10 h-10 rounded-full bg-primary/10 flex items-center justify-center text-primary mr-4">
                                    <i class="fa fa-phone"></i>
                                </div>
                                <div>
                                    <h4 class="font-bold text-neutral-800 mb-1">电话</h4>
                                    <p class="text-neutral-600">+86 021-12345678</p>
                                </div>
                            </div>
                            
                            <div class="flex items-start">
                                <div class="w-10 h-10 rounded-full bg-primary/10 flex items-center justify-center text-primary mr-4">
                                    <i class="fa fa-envelope"></i>
                                </div>
                                <div>
                                    <h4 class="font-bold text-neutral-800 mb-1">邮箱</h4>
                                    <p class="text-neutral-600">example@mail.com</p>
                                </div>
                            </div>
                        </div>
                        
                        <div class="mt-8">
                            <h4 class="font-bold text-neutral-800 mb-3">关注我们</h4>
                            <div class="flex space-x-4">
                                <a href="#" class="w-10 h-10 rounded-full bg-primary/10 flex items-center justify-center text-primary hover:bg-primary hover:text-white transition-colors">
                                    <i class="fa fa-weixin"></i>
                                </a>
                                <a href="#" class="w-10 h-10 rounded-full bg-primary/10 flex items-center justify-center text-primary hover:bg-primary hover:text-white transition-colors">
                                    <i class="fa fa-twitter"></i>
                                </a>
                                <a href="#" class="w-10 h-10 rounded-full bg-primary/10 flex items-center justify-center text-primary hover:bg-primary hover:text-white transition-colors">
                                    <i class="fa fa-linkedin"></i>
                                </a>
                                <a href="#" class="w-10 h-10 rounded-full bg-primary/10 flex items-center justify-center text-primary hover:bg-primary hover:text-white transition-colors">
                                    <i class="fa fa-youtube"></i>
                                </a>
                            </div>
                        </div>
                    </div>
                    
                    <div>
                        <h3 class="text-xl font-bold text-neutral-800 mb-4">发送消息</h3>
                        
                        <form>
                            <div class="mb-4">
                                <label for="name" class="block text-sm font-medium text-neutral-700 mb-1">姓名</label>
                                <input type="text" id="name" class="w-full px-3 py-2 border border-neutral-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-primary/50 focus:border-primary">
                            </div>
                            
                            <div class="mb-4">
                                <label for="email" class="block text-sm font-medium text-neutral-700 mb-1">邮箱</label>
                                <input type="email" id="email" class="w-full px-3 py-2 border border-neutral-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-primary/50 focus:border-primary">
                            </div>
                            
                            <div class="mb-4">
                                <label for="subject" class="block text-sm font-medium text-neutral-700 mb-1">主题</label>
                                <input type="text" id="subject" class="w-full px-3 py-2 border border-neutral-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-primary/50 focus:border-primary">
                            </div>
                            
                            <div class="mb-6">
                                <label for="message" class="block text-sm font-medium text-neutral-700 mb-1">消息内容</label>
                                <textarea id="message" rows="4" class="w-full px-3 py-2 border border-neutral-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-primary/50 focus:border-primary resize-none"></textarea>
                            </div>
                            
                            <button type="submit" class="w-full bg-primary text-white py-2 px-4 rounded-lg hover:bg-primary/90 transition-colors">
                                发送消息
                            </button>
                        </form>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- 页脚 -->
    <footer class="bg-neutral-800 text-white py-10">
        <div class="container mx-auto px-4">
            <div class="flex flex-col md:flex-row justify-between items-center">
                <div class="mb-6 md:mb-0">
                    <div class="flex items-center justify-center md:justify-start">
                        <div class="w-10 h-10 rounded-full bg-white flex items-center justify-center text-primary mr-3">
                            <i class="fa fa-flask"></i>
                        </div>
                        <span class="text-xl font-bold">环境感知与建模研究组</span>
                    </div>
                    <p class="text-neutral-400 mt-2 text-center md:text-left">
                        致力于环境科学与技术领域的前沿研究
                    </p>
                </div>
                
                <div class="text-center md:text-right">
                    <p class="text-neutral-400">© 2023 环境感知与建模研究组. 保留所有权利.</p>
                    <p class="text-neutral-400 mt-1">
                        <a href="#" class="hover:text-white transition-colors">隐私政策</a> · 
                        <a href="#" class="hover:text-white transition-colors">使用条款</a> · 
                        <a href="#" class="hover:text-white transition-colors">网站地图</a>
                    </p>
                </div>
            </div>
        </div>
    </footer>

    <!-- JavaScript -->
    <script>
        // 移动端菜单切换
        const menuToggle = document.getElementById('menu-toggle');
        const mobileMenu = document.getElementById('mobile-menu');
        
        menuToggle.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
        });
        
        // 平滑滚动
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                
                // 关闭移动端菜单
                if (!mobileMenu.classList.contains('hidden')) {
                    mobileMenu.classList.add('hidden');
                }
                
                const targetId = this.getAttribute('href');
                const targetElement = document.querySelector(targetId);
                
                if (targetElement) {
                    window.scrollTo({
                        top: targetElement.offsetTop - 80,
                        behavior: 'smooth'
                    });
                }
            });
        });
        
        // 导航栏滚动效果
        const header = document.querySelector('header');
        let lastScrollY = window.scrollY;
        
        window.addEventListener('scroll', () => {
            if (window.scrollY > 100) {
                header.classList.add('py-2');
                header.classList.remove('py-4');
                header.classList.add('shadow-lg');
            } else {
                header.classList.remove('py-2');
                header.classList.add('py-4');
                header.classList.remove('shadow-lg');
            }
            
            lastScrollY = window.scrollY;
        });
    </script>
</body>
</html>
    
