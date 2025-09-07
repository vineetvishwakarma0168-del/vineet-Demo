# vineet-Demo
This is my first git repository .
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>GitHub Inspired Page</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
        }
        
        body {
            background-color: #0d1117;
            color: #c9d1d9;
            line-height: 1.5;
        }
        
        .container {
            max-width: 1280px;
            margin: 0 auto;
            padding: 0 16px;
        }
        
        /* Header */
        header {
            background-color: #161b22;
            padding: 12px 0;
            border-bottom: 1px solid #30363d;
        }
        
        .header-content {
            display: flex;
            align-items: center;
            justify-content: space-between;
        }
        
        .logo {
            display: flex;
            align-items: center;
            gap: 16px;
        }
        
        .logo svg {
            fill: #f0f6fc;
        }
        
        .search-bar {
            background-color: #0d1117;
            border: 1px solid #30363d;
            border-radius: 6px;
            padding: 8px 16px;
            color: #c9d1d9;
            width: 300px;
            margin: 0 16px;
        }
        
        .nav-links {
            display: flex;
            gap: 16px;
        }
        
        .nav-links a {
            color: #c9d1d9;
            text-decoration: none;
            font-weight: 500;
        }
        
        .nav-links a:hover {
            color: #f0f6fc;
        }
        
        /* Main Content */
        .main-content {
            display: flex;
            margin-top: 32px;
            gap: 16px;
        }
        
        .profile-section {
            width: 25%;
        }
        
        .profile-card {
            background-color: #161b22;
            border: 1px solid #30363d;
            border-radius: 6px;
            padding: 16px;
            text-align: center;
        }
        
        .profile-img {
            width: 100%;
            border-radius: 50%;
            max-width: 200px;
            border: 1px solid #30363d;
        }
        
        .profile-name {
            margin-top: 16px;
            font-size: 24px;
            font-weight: 600;
        }
        
        .profile-username {
            color: #7d8590;
            font-size: 18px;
        }
        
        .profile-bio {
            margin: 16px 0;
        }
        
        .profile-stats {
            display: flex;
            justify-content: center;
            gap: 16px;
            margin: 16px 0;
        }
        
        .profile-stat {
            display: flex;
            align-items: center;
            gap: 4px;
        }
        
        /* Repositories */
        .repos-section {
            width: 75%;
        }
        
        .repos-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 16px;
        }
        
        .section-title {
            font-size: 24px;
            font-weight: 600;
        }
        
        .repo-filters {
            display: flex;
            gap: 8px;
        }
        
        .btn {
            background-color: #21262d;
            color: #c9d1d9;
            border: 1px solid #30363d;
            border-radius: 6px;
            padding: 8px 16px;
            cursor: pointer;
            font-weight: 500;
            display: flex;
            align-items: center;
            gap: 4px;
        }
        
        .btn-primary {
            background-color: #238636;
            color: #fff;
            border: 1px solid #2ea043;
        }
        
        .btn-primary:hover {
            background-color: #2ea043;
        }
        
        .btn:hover {
            background-color: #30363d;
        }
        
        .repo-list {
            display: flex;
            flex-direction: column;
            gap: 16px;
        }
        
        .repo-card {
            background-color: #161b22;
            border: 1px solid #30363d;
            border-radius: 6px;
            padding: 16px;
        }
        
        .repo-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 8px;
        }
        
        .repo-name {
            color: #58a6ff;
            text-decoration: none;
            font-weight: 600;
            font-size: 18px;
        }
        
        .repo-name:hover {
            text-decoration: underline;
        }
        
        .repo-visibility {
            border: 1px solid #30363d;
            border-radius: 12px;
            padding: 2px 8px;
            font-size: 12px;
            color: #7d8590;
        }
        
        .repo-desc {
            margin-bottom: 16px;
            color: #7d8590;
        }
        
        .repo-details {
            display: flex;
            gap: 16px;
            color: #7d8590;
            font-size: 14px;
        }
        
        .repo-detail {
            display: flex;
            align-items: center;
            gap: 4px;
        }
        
        /* Footer */
        footer {
            margin-top: 40px;
            padding: 24px 0;
            border-top: 1px solid #30363d;
            text-align: center;
            color: #7d8590;
        }
        
        .footer-links {
            display: flex;
            justify-content: center;
            gap: 16px;
            margin-top: 8px;
        }
        
        .footer-links a {
            color: #58a6ff;
            text-decoration: none;
        }
        
        .footer-links a:hover {
            text-decoration: underline;
        }
        
        /* Responsive */
        @media (max-width: 768px) {
            .main-content {
                flex-direction: column;
            }
            
            .profile-section, .repos-section {
                width: 100%;
            }
            
            .header-content {
                flex-direction: column;
                gap: 16px;
            }
            
            .search-bar {
                width: 100%;
                margin: 0;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="container">
            <div class="header-content">
                <div class="logo">
                    <svg height="32" aria-hidden="true" viewBox="0 0 16 16" version="1.1" width="32" data-view-component="true">
                        <path d="M8 0C3.58 0 0 3.58 0 8C0 11.54 2.29 14.53 5.47 15.59C5.87 15.66 6.02 15.42 6.02 15.21C6.02 15.02 6.01 14.39 6.01 13.72C4 14.09 3.48 13.23 3.32 12.78C3.23 12.55 2.84 11.84 2.5 11.65C2.22 11.5 1.82 11.13 2.49 11.12C3.12 11.11 3.57 11.7 3.72 11.94C4.44 13.15 5.59 12.81 6.05 12.6C6.12 12.08 6.33 11.73 6.56 11.53C4.78 11.33 2.92 10.64 2.92 7.58C2.92 6.71 3.23 5.99 3.74 5.43C3.66 5.23 3.38 4.41 3.82 3.31C3.82 3.31 4.49 3.1 6.02 4.13C6.66 3.95 7.34 3.86 8.02 3.86C8.7 3.86 9.38 3.95 10.02 4.13C11.55 3.09 12.22 3.31 12.22 3.31C12.66 4.41 12.38 5.23 12.3 5.43C12.81 5.99 13.12 6.7 13.12 7.58C13.12 10.65 11.25 11.33 9.47 11.53C9.76 11.78 10.01 12.26 10.01 13.01C10.01 14.08 10 14.94 10 15.21C10 15.42 10.15 15.67 10.55 15.59C13.71 14.53 16 11.53 16 8C16 3.58 12.42 0 8 0Z"></path>
                    </svg>
                </div>
                
                <input type="text" class="search-bar" placeholder="Search or jump to...">
                
                <div class="nav-links">
                    <a href="#">Pull requests</a>
                    <a href="#">Issues</a>
                    <a href="#">Codespaces</a>
                    <a href="#">Marketplace</a>
                    <a href="#">Explore</a>
                </div>
            </div>
        </div>
    </header>
    
    <div class="container">
        <main class="main-content">
            <section class="profile-section">
                <div class="profile-card">
                    <img src="https://via.placeholder.com/260" alt="Profile Image" class="profile-img">
                    <h1 class="profile-name">John Doe</h1>
                    <p class="profile-username">johndoe</p>
                    <p class="profile-bio">Software developer passionate about open source and web technologies.</p>
                    
                    <div class="profile-stats">
                        <div class="profile-stat">
                            <i class="fas fa-users"></i>
                            <span>24 followers</span>
                        </div>
                        <div class="profile-stat">
                            <span>·</span>
                            <span>15 following</span>
                        </div>
                    </div>
                    
                    <div class="profile-stats">
                        <div class="profile-stat">
                            <i class="fas fa-map-marker-alt"></i>
                            <span>San Francisco, CA</span>
                        </div>
                    </div>
                </div>
            </section>
            
            <section class="repos-section">
                <div class="repos-header">
                    <h2 class="section-title">Repositories</h2>
                    <div class="repo-filters">
                        <button class="btn">
                            <i class="fas fa-filter"></i>
                            <span>Filters</span>
                        </button>
                        <button class="btn btn-primary">
                            <i class="fas fa-plus"></i>
                            <span>New</span>
                        </button>
                    </div>
                </div>
                
                <div class="repo-list">
                    <div class="repo-card">
                        <div class="repo-header">
                            <a href="#" class="repo-name">awesome-project</a>
                            <span class="repo-visibility">Public</span>
                        </div>
                        <p class="repo-desc">A curated list of awesome resources and projects.</p>
                        <div class="repo-details">
                            <div class="repo-detail">
                                <span style="color: #f34f29;">●</span>
                                <span>HTML</span>
                            </div>
                            <div class="repo-detail">
                                <i class="far fa-star"></i>
                                <span>128</span>
                            </div>
                            <div class="repo-detail">
                                <i class="fas fa-code-branch"></i>
                                <span>12</span>
                            </div>
                            <div class="repo-detail">
                                <span>Updated 3 days ago</span>
                            </div>
                        </div>
                    </div>
                    
                    <div class="repo-card">
                        <div class="repo-header">
                            <a href="#" class="repo-name">node-backend</a>
                            <span class="repo-visibility">Public</span>
                        </div>
                        <p class="repo-desc">A backend server built with Node.js and Express.</p>
                        <div class="repo-details">
                            <div class="repo-detail">
                                <span style="color: #f1e05a;">●</span>
                                <span>JavaScript</span>
                            </div>
                            <div class="repo-detail">
                                <i class="far fa-star"></i>
                                <span>42</span>
                            </div>
                            <div class="repo-detail">
                                <i class="fas fa-code-branch"></i>
                                <span>7</span>
                            </div>
                            <div class="repo-detail">
                                <span>Updated 2 weeks ago</span>
                            </div>
                        </div>
                    </div>
                    
                    <div class="repo-card">
                        <div class="repo-header">
                            <a href="#" class="repo-name">react-ui-library</a>
                            <span class="repo-visibility">Private</span>
                        </div>
                        <p class="repo-desc">A collection of reusable React components.</p>
                        <div class="repo-details">
                            <div class="repo-detail">
                                <span style="color: #61dafb;">●</span>
                                <span>TypeScript</span>
                            </div>
                            <div class="repo-detail">
                                <i class="far fa-star"></i>
                                <span>86</span>
                            </div>
                            <div class="repo-detail">
                                <i class="fas fa-code-branch"></i>
                                <span>9</span>
                            </div>
                            <div class="repo-detail">
                                <span>Updated 5 days ago</span>
                            </div>
                        </div>
                    </div>
                </div>
            </section>
        </main>
    </div>
    
    <footer>
        <div class="container">
            <p>© 2023 GitHub, Inc.</p>
            <div class="footer-links">
                <a href="#">Terms</a>
                <a href="#">Privacy</a>
                <a href="#">Security</a>
                <a href="#">Status</a>
                <a href="#">Docs</a>
                <a href="#">Contact</a>
            </div>
        </div>
    </footer>

    <script>
        // Simple JavaScript for demonstration
        document.querySelector('.btn-primary').addEventListener('click', function() {
            alert('This would normally open a repository creation dialog.');
        });
    </script>
</body>
</html>
Author - VineetVishwakarma 
