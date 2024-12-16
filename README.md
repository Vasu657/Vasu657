import React, { useState } from 'react'
import { Sun, Moon, CodeIcon, DatabaseIcon, CloudIcon, TerminalIcon } from 'lucide-react'

const GithubProfile = () => {
  const [isDarkMode, setIsDarkMode] = useState(true)

  const toggleTheme = () => {
    setIsDarkMode(!isDarkMode)
  }

  const themeClasses = isDarkMode 
    ? 'bg-[#0D1117] text-white' 
    : 'bg-white text-black'

  const skills = [
    { 
      icon: <DatabaseIcon className="mr-2" />, 
      name: 'Data Analysis', 
      tools: ['Power BI', 'SQL', 'Python', 'Excel'] 
    },
    { 
      icon: <CloudIcon className="mr-2" />, 
      name: 'Cloud & DevOps', 
      tools: ['AWS', 'Docker', 'Jenkins', 'Kubernetes'] 
    },
    { 
      icon: <CodeIcon className="mr-2" />, 
      name: 'Programming', 
      tools: ['Python', 'SQL', 'VBA', 'Full-Stack Web Dev'] 
    }
  ]

  return (
    <div 
      className={`min-h-screen p-8 transition-all duration-300 ${themeClasses}`}
    >
      <div className="max-w-4xl mx-auto">
        {/* Theme Toggle */}
        <button 
          onClick={toggleTheme} 
          className="absolute top-4 right-4 hover:rotate-180 transition-transform"
        >
          {isDarkMode ? <Sun color="orange" /> : <Moon color="purple" />}
        </button>
        {/* Header */}
        <div className="text-center mb-10">
          <h1 className="text-4xl font-bold mb-2">
            Vasu Ghanta 
            <span className="text-lg ml-2 text-gray-500">
              Data Analyst & DevOps Engineer
            </span>
          </h1>
          <p className="text-xl text-gray-400">
            Transforming Data into Actionable Insights
          </p>
        </div>
        {/* About Me */}
        <div className="mb-10 bg-gray-800 p-6 rounded-lg">
          <h2 className="text-2xl font-semibold mb-4 flex items-center">
            <TerminalIcon className="mr-3" />
            About Me
          </h2>
          <p>
            Passionate Data Analyst and AWS DevOps enthusiast with expertise in 
            optimizing healthcare analytics, automating workflows, and driving 
            data-driven decision-making. Skilled in transforming complex data 
            into meaningful insights using cutting-edge technologies.
          </p>
        </div>
        {/* Top Skills */}
        <div className="grid md:grid-cols-3 gap-6">
          {skills.map((skill, index) => (
            <div 
              key={index} 
              className="bg-gray-800 p-6 rounded-lg hover:scale-105 transition-transform"
            >
              <div className="flex items-center mb-4">
                {skill.icon}
                <h3 className="text-xl font-semibold">{skill.name}</h3>
              </div>
              <div className="flex flex-wrap gap-2">
                {skill.tools.map((tool, toolIndex) => (
                  <span 
                    key={toolIndex} 
                    className="bg-blue-600 text-white px-3 py-1 rounded-full text-sm"
                  >
                    {tool}
                  </span>
                ))}
              </div>
            </div>
          ))}
        </div>
        {/* Social Links */}
        <div className="flex justify-center mt-10 space-x-4">
          <a 
            href="https://www.linkedin.com/in/vasu-ghanta" 
            target="_blank" 
            className="hover:scale-110 transition-transform"
          >
            <img 
              src="/api/placeholder/40/40" 
              alt="LinkedIn" 
              className="w-10 h-10 bg-blue-600 rounded-full"
            />
          </a>
          <a 
            href="https://vasu-ghanta.web.app/" 
            target="_blank" 
            className="hover:scale-110 transition-transform"
          >
            <img 
              src="/api/placeholder/40/40" 
              alt="Portfolio" 
              className="w-10 h-10 bg-green-600 rounded-full"
            />
          </a>
          <a 
            href="mailto:vasughanta2k@gmail.com" 
            className="hover:scale-110 transition-transform"
          >
            <img 
              src="/api/placeholder/40/40" 
              alt="Email" 
              className="w-10 h-10 bg-red-600 rounded-full"
            />
          </a>
        </div>
      </div>
    </div>
  )
}

export default GithubProfile
