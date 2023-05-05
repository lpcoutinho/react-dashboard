1. npx create-react-app ./
2. delete and create src/
    - create new App.js
        - use snippet `rafce`
    - create new index.js
3. install dependencies `npm install`
4. create index.css
5. create App.css
6. https://tailwindcss.com/docs/guides/create-react-app
7. create tailwind.config.js
8. create craco.config.js
9. create folders: components, contexts, pages
10. create folder data and populete it
11. create dammy.js in /data
12. create BrowserRouter
    - div className="flex relative dark:bg-main-dark-bg"
    - <div className="fixed right-4 bottom-4" style={{ zIndex: '1000' }}>
13. create TooltipComponent
    - <TooltipComponent content="Settings" position="Top">
14. create button with FiSettings
15. npm start to see the settings button on the right corner of the page
16. edite button
    -  <button type='button' 
            className='text-3x1 p-3 hover:drop-shadow-x1 hover:bg-light-gray text-white'
            style={{background: 'blue', borderRadius: '50%'}}>
17. create activeMenu for Sidebar
    - {activeMenu ? (
          <div>
            Sidebar
          </div>
        ) : (
          <div>
            Sidebar w-0
          </div>
        )}
18. create a const for this sidebar
    -   const activeMenu = true
19. edite divs from activeMenu sidebar
    -           <div className='w-72 fixed sidebar dark:bg-secondary-dark-bg bg-white'>
    -             <div className='w-0 dark:bg-secondary-dark-bg'>

20. create div to show or not sidebar
    - https://tailwindcss.com/docs/width
        <div className={`dark:bg-main-bg bg-main-bg main-h-screen w-full ${activeMenu ? 'md:ml-72' :'flex-2'}`}>
    - 
21. create div do show Navbar
    - <div className='fixed md:static bg-main-bg dark:bg-main-dark-bg navbar w-full '>
            Navbar
          </div>
22. create Routes
23. create components/Button.jsx, Cart.jsx, Chat.jsx, ChartsHeader.jsx, Footer.jsx, Header.jsx, Navbar.jsx, Notification.jsx, Sidebar.jsx, ThemeSettings.jsx, UserProfile.jsx
    - use snippet rafce
24. create components/Charts/LineChart.jsx, Pie.jsx, SparkLine.jsx, Stacked.jsx
    - use snippet rafce
25. create components/index.jsx
    - export all components
26. create pages/Calendar.jsx, ColorPicker.jsx, Customers.jsx, Ecommerce.jsx, Editor.jsx, Employees.jsx, Kanban.jsx, Orders.jsx, 
    - use snippet rafce
27.  create pages/Charts/Area.jsx, Bar.jsx, ColorMapping.jsx, Financial.jsx, Line.jsx, Pie.jsx, Pyramid.jsx, Stacked.jsx
    - use snippet rafce
28. create pages/index.jsx
    - export all components
29. import components & pages in APP.js
30. insert components navbar & sidebar in your divs
31 . update element in Routes to receive components
32. git push
############# build sidebar #############
33. import { Link, NavLink } from 'react-router-dom';import { SiShopware } from 'react-icons/si';
import { MdOutlineCancel } from 'react-icons/md'; import { TooltipComponent } from '@syncfusion/ej2-react-popups'; import { links } from '../data/dummy';
34. create const activeMenu
35. create activeMenu and a link whith icon and text
    - { activeMenu && (
        <>
          <div className="flex justify-between items-center">
            <Link to="/" onClick={() => {}} className="items-center gap-3 ml-3 mt-4 flex text-xl font-extrabold tracking-tight dark:text-white text-slate-900">
              <SiShopware /> <span>Teste</span>
            </Link>
          </div>
        </>
      )}
36. create a TooltipComponent and a button MdOutlineCancel inside it
37. create the links with `map`
38. create activeLink & normalLink
39. create context/ContextProvider.js
40. create context to activemenu
41. edite index.js to import ContextProvider and add to reactDOM
    - ReactDOM.render(
    <ContextProvider>
        <App />
    </ContextProvider>,
    document.getElementById('root')
);
42. update const activeMenu in App.js
    - const { activeMenu } = useStateContext();
43. update Sidebar to import { useStateContext } from './contexts/ContextProvider'

44. update ContextProvider.js to receive setActiveMenu
45. update Sidebar.js to   const { activeMenu, setActiveMenu } = useStateContext();
46. update Sidebar.js to setActiveMenu
47. 
48. 
49. 
50. 
51. 